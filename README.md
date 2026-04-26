🚚 UniUni 运输数据自动填表工具 | UniUni Auto-Filler Tool

🌟 核心功能
多格式兼容：自动识别带路线前缀（如 936EWR-ORD）、四位年份、英文星期等复杂文本。

逻辑安全校验：自动检查时间顺序，确保 “卸货时间 > 到达时间 > 发车时间”。若顺序异常，工具会变红预警。

零插件运行：生成纯脚本代码，通过浏览器控制台执行，无需安装任何插件。

🚀 使用指南
解析数据：打开工具网页（index.html），将包含 BOL# 的原始文本粘贴到输入框，点击 “解析并检查逻辑”。

获取脚本：确认预览表无误后，点击底部的 “复制全部代码”。

自动填充：

登录 UniUni 后台，进入对应页面。

按下 F12 或右键选择 “检查” (Inspect)。

切换到 Console (控制台) 选项卡。

粘贴代码 (Ctrl+V) 并按 Enter。

⚠️ 注意事项
核对数据：提交前请抽查前几行，确保填充位置准确。

列数定位：默认填充第 8 列（到达）和第 9 列（卸货）。若页面改版，需微调代码中的 nth-child。

🌟 Key Features
Format Compatibility: Automatically recognizes complex text containing route prefixes (e.g., 936EWR-ORD), 4-digit years, and English weekdays.

Logic Validation: Automatically verifies time sequence: "Unload Time > Arrival Time > Departure Time". Errors are highlighted in red.

Plugin-Free: Generates pure JavaScript for browser console execution—no third-party extensions required.

🚀 How to Use
Parse Data: Open the tool (index.html), paste raw text with BOL# info into the box, and click "Analyze & Verify Logic".

Get Script: Once verified in the preview table, click "Copy All Code" at the bottom.

Auto-Fill:

Log in to the UniUni Portal and navigate to the target page.

Press F12 or right-click and select "Inspect".

Switch to the Console tab.

Paste the code (Ctrl+V) and hit Enter.

⚠️ Important Notes
Data Verification: Please double-check the first few rows before clicking "Submit" on the portal.

Column Mapping: Default mapping is Column 8 (Arrival) and Column 9 (Unload). If the portal layout changes, update the nth-child index in the script.

🛠️ Developer Info
Repo: czb135/936_filler

Stack: HTML5, CSS3, Vanilla JavaScript (Regex-based parsing).
