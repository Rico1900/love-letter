# Love Letter (LaTeX)

这是一个使用 LaTeX 排版的情书项目，当前文件为英文草稿，计划改写为中文正式版。

## 文件结构
- `main.tex`：情书主文档
- `AGENTS.md`：后续协作编辑规范
- `.gitignore`：LaTeX 构建产物忽略规则

## 环境要求
- 推荐 TeX Live / MacTeX（需包含 `ctex`、`tikz`、`pgfornament`）
- 使用 `xelatex` 编译（中文支持更稳定）

## 编译命令
```bash
xelatex -interaction=nonstopmode -halt-on-error main.tex
xelatex -interaction=nonstopmode -halt-on-error main.tex
```

编译成功后会生成 `main.pdf`。

## 英文转中文建议流程
1. 先保留原段落结构，逐段翻译，保证语义对齐。
2. 将英文标点全部替换为中文标点，统一语气和称呼。
3. 通读一遍，重点检查：
   - 情感是否自然，不生硬直译
   - 中文断句是否顺口
   - 是否出现过长行导致视觉拥挤
4. 编译 PDF 做最终校对。

## 可选下一步
- 如需保留英文底稿，可复制 `main.tex` 为 `main.en.tex`。
- 如需中英双语版，可将中文正文放在英文段落后并加入适度留白。
