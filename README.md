# my-docs

使用 MkDocs Material 搭建的个人文档网站，通过 GitHub Actions 自动构建并部署到 GitHub Pages。

## 链接

- 网站地址：https://czx666859.github.io/my-docs/
- [个人实验报告](report/README.md)

## 本地预览

```bash
python -m venv .venv
python -m pip install -r requirements.txt
python -m mkdocs build --strict
python -m mkdocs serve
```

启动后访问 `http://127.0.0.1:8000/my-docs/`，检查完成后按 `Ctrl+C` 停止。