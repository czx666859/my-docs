# 使用指南

1. 修改 docs 目录中的 Markdown 文件。
2. 在本地预览并检查页面及链接。
3. 提交修改并推送到 main 分支。
4. 在 Actions 页面查看构建与部署状态。
5. 打开网站检查内容是否更新。

## 常用命令

- python -m mkdocs serve：本地预览。
- python -m mkdocs build --strict：构建网站并严格检查警告。

## 本地预览示例

```bash
python -m venv .venv
python -m pip install -r requirements.txt
python -m mkdocs build --strict
python -m mkdocs serve
```

## 我在实践中注意到的几点

- 因为配置了 `site_url`，本地预览的地址不是 `http://127.0.0.1:8000/`，而是 `http://127.0.0.1:8000/my-docs/`，和线上网站的路径保持一致。
- 构建时加上 `--strict`，出现任何警告都会失败，能在推送之前就发现失效链接之类的问题。
- 我本地使用的 Python 是 3.14，而云端工作流指定的是 3.12。两者都能成功构建，说明这个项目对 Python 小版本不敏感。
- 构建时终端会打印主题的维护公告，它只是提示，不影响构建结果。

想了解项目背景，请阅读 [关于本项目](about.md)；接口示例见 [API 参考](api.md)。