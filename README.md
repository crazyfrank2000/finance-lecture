# 金融学讲义 (Finance Lecture)

这是一个使用LaTeX编写的金融学讲义项目，采用ElegantBook文档类，支持中文排版。

## 📚 项目简介

本项目包含完整的金融学课程讲义，分为5个主要章节，使用专业的LaTeX排版系统制作。

## 📁 文件结构

```
Finance_lec/
├── main.tex                 # 主文档文件
├── 1.tex                    # 第一章内容
├── 2.tex                    # 第二章内容  
├── 3.tex                    # 第三章内容
├── 4.tex                    # 第四章内容
├── 5.tex                    # 第五章内容
├── newcommand.tex           # 自定义命令和宏
├── reference.bib            # 参考文献数据库
├── 0-figure/                # 样式和资源文件
│   ├── cover.png            # 封面图片
│   ├── elegantbook.cls      # ElegantBook文档类
│   ├── extraenv.sty         # 额外环境定义
│   └── extrarelation.sty    # 额外关系定义
├── figure/                  # 图片文件夹
└── SourceHanFonts/          # 思源字体文件
    └── OTF/SimplifiedChinese/  # 简体中文字体
```

## 🔧 编译要求

### 系统要求
- **TeX发行版**: TeX Live 2020+ 或 MiKTeX
- **编译引擎**: XeLaTeX (推荐) 或 LuaLaTeX
- **参考文献处理**: Biber

### 字体要求
项目已包含思源字体文件，支持中文显示：
- Source Han Sans SC (思源黑体)

## 🚀 编译方法

### 方法一：完整编译 (推荐)
```bash
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex
```

### 方法二：使用latexmk自动编译
```bash
latexmk -xelatex -biber main.tex
```

### 方法三：VS Code + LaTeX Workshop
1. 安装LaTeX Workshop扩展
2. 打开main.tex文件
3. 使用快捷键 `Ctrl+Alt+B` 编译

## 📖 使用说明

1. **编辑内容**: 主要内容分布在`1.tex`到`5.tex`文件中
2. **添加图片**: 将图片放入`figure/`文件夹并在相应章节中引用
3. **自定义命令**: 在`newcommand.tex`中添加常用的数学公式和命令
4. **参考文献**: 在`reference.bib`中添加文献条目

## 📝 章节内容

- **第1章**: [章节主题]
- **第2章**: [章节主题]  
- **第3章**: [章节主题]
- **第4章**: [章节主题]
- **第5章**: [章节主题]

## 🛠️ 开发环境建议

### 推荐编辑器
- **VS Code** + LaTeX Workshop扩展
- **TeXstudio**
- **Overleaf** (在线编辑)

### 编译配置
建议在编辑器中设置XeLaTeX为默认编译引擎，以获得最佳的中文支持。

## 📄 输出文件

编译成功后会生成`main.pdf`文件，这是最终的讲义文档。

## 🔍 故障排除

### 常见问题
1. **中文显示异常**: 确保使用XeLaTeX编译
2. **参考文献不显示**: 运行biber命令处理参考文献
3. **字体错误**: 检查SourceHanFonts文件夹是否完整

### 清理编译文件
```bash
# 删除编译产物，保留源文件和PDF
rm -f *.aux *.log *.out *.toc *.bcf *.run.xml *.fdb_latexmk *.fls *.synctex.gz
```

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个项目。

## 📜 许可证

本项目采用 [MIT License](LICENSE)。

## 📧 联系方式

如有问题请通过GitHub Issues联系。

---

*使用ElegantBook文档类制作 | 支持中文排版 | LaTeX驱动* 