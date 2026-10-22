教材智能点读助手（网页原型）
================================

这是第一版静态网页，可部署到 Cloudflare Pages，无需在个人电脑安装 Python。

当前功能：
- 浏览器内打开 PDF 和图片
- 读取 TXT 文本并点击文字朗读
- 使用设备/浏览器提供的语音
- 适配电脑和手机屏幕

当前限制：
- 尚未集成 OCR，所以扫描版 PDF、图片不会自动识别文字
- DOCX 解析暂未实现，请暂时另存为 PDF 或 TXT
- PDF 当前为原始页面预览，尚未实现 PDF 文字位置点击朗读
- 此版本不把文件上传到服务器；文件只在当前浏览器中处理
- 云端 OCR、云端语音和账号/教材库功能需后续开发

Cloudflare Pages 部署：
1. 解压 ZIP。
2. 登录 Cloudflare Dashboard。
3. 打开 Workers & Pages / Pages。
4. 选择创建应用，选择上传静态资源（Direct Upload / Upload assets；具体名称可能随界面更新）。
5. 上传解压后包含 index.html 的文件夹，或按页面提示上传文件。
6. 发布成功后访问 Cloudflare 提供的 *.pages.dev 地址。

注意：不要把教材、密码、API Key 上传到 GitHub 公共仓库。
