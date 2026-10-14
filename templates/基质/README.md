# 基质识别模板

来源：Logical-Byte/endfield-essence-recognizer，commit `066d0e5b830fa06e0addbb52966fe6513b7e4eb1`。

- 31 张词条：`src/endfield_essence_recognizer/templates/generated/<词条 ID>.png`。
- 5 张界面模板：`templates/screenshot/` 下的「武器基质」「已锁定」「未锁定」「已弃用」「未弃用」。
- 转换：原图转 RGB，宽高乘 `2/3` 后四舍五入，以双线性滤波缩放到 720p。
- 对应布局：OEA `src-tauri/src/automation/essence_scan/layout.rs`，参考 EER `core/layout/res_1080p.py`。

该目录保留上游 `LICENSE` 为 `LICENSE.EER`。游戏图像的来源归属保持不变。
缩放模板尚需 Windows 720p 实机校准，人工合成截图只验证匹配管线。
