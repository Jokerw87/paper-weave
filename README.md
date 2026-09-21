# 纸上编织实验室 / Paper Weave

An original, local visual repeat-pattern experiment. Open `index.html` with all files in one folder. No server, external fonts, account, upload or persistent storage.

## 三步使用

1. 选择单元大小和起始图案，点击“应用起始图案”。这两个选择只用于下一次应用，不会立即改变当前作品。配色会立即应用。
2. 点击交叠格，或 Tab 进入后用方向键和空格/Enter 编辑。实心代表竖条在上，空心代表横条在上。查看右侧三乘三平铺与接缝统计。
3. 保存 JSON 以便继续编辑；下载 SVG 或 1200×1200 PNG 作为图案。保存按钮只能请求浏览器下载，请自行确认文件落盘。

支持 4、6、8、12 格单元，三组固定配色，最多100步撤销。应用预设或导入覆盖编辑内容前会询问；导入完成后可撤销。JSON须为32 KiB以内的本工具格式，读取过程中若图案改变，不会用迟到文件覆盖新状态。关闭或刷新会丢失未保存作品。

## 统计含义

单元内最长：一行或一列中连续相同状态的最长长度。跨接缝最长：该行/列首尾连接后的连续长度。整条线只有一种状态时，在无限重复下为“无限”，不是单元边长。两种状态、两个方向均计入；这不是某一布料表面的专业浮线鉴定。

示意预设名称仅描述图形。6格与4格周期的图案相遇时接缝可能不同，这正是要观察的内容。SVG/PNG只画纸条示意，不包含诊断表；诊断表位于页面。

## Boundaries

Not loom-control software, WIF, fabric simulation, manufacturability or safety validation. No material thickness, tension, shrinkage or construction calculation. Existing richer weaving tools include Woven Images and Loom Logic; this is a personal creative/learning artifact, not a novel or market-validated product. No third-party source copied. No reuse license selected in this initial publication.

## Tests

Run `node test-engine.cjs`. With an existing Playwright installation, set `PLAYWRIGHT_MODULE` to its module path, then run `node test-browser.cjs` or `node test-boundaries.cjs`. Generated evidence folders are not distribution source. See TEST_RESULTS.md for actual scope.
