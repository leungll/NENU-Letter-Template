<!--
 * @Author: Lili Liang
 * @Date: 2024-05-19 21:22:15
 * @LastEditors: Lili Liang
 * @LastEditTime: 2024-05-24 13:55:33
 * @Description: Please set description
-->
# NENU-Letter-Template
NENU's recommendation letter template.

东北师范大学推荐信模板

![Author](https://img.shields.io/badge/Author-Lili_Liang-red)
![GitHub last commit](https://img.shields.io/github/last-commit/leungll/NENU-Letter-Template?color=yellow)
![GitHub repo size](https://img.shields.io/github/repo-size/leungll/NENU-Letter-Template)
![Static Badge](https://img.shields.io/badge/language-latex-orange)
![GitHub License](https://img.shields.io/github/license/leungll/NENU-Letter-Template?color=green)

## 示例
![NENU-Letter](https://cdn.jsdelivr.net/gh/leungll/MyImgHosting/img/NENU-Letter.png) | ![CMU-Letter](https://cdn.jsdelivr.net/gh/leungll/MyImgHosting/img/CMU-Letter.png)
---|---

## 特性
- **无需了解太多的 [Latex](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes) 语法即可使用该模板**
- 支持使用 [Overleaf](https://www.overleaf.com/latex/templates/nenu-letter-template/fvqdkcyhnbsv) 在线编译，无需安装 [TexLive](https://tug.org/texlive) 本地环境
- 一个简单的模板，可进一步定制或扩展
- 将推荐信内容和模板框架进行分离
- 支持在生成的 PDF 中添加超链接，例如电子邮件或 URL
- 支持添加脚注

## 项目结构
```
.
├── LICENSE                 \\ repo license
├── README.md               \\ readme in Chinese
├── letterContent.tex       \\ main content of the letter, isolates from the template frame
├── main.pdf                \\ letter pdf generated after latex compilation
├── main.tex                \\ template frame
├── pic                     \\ folder where pictures are stored
│   ├── NENU_Logo.png
│   ├── NENU_Logo_Bg.png
│   └── signature.png
└── sample                  \\ sample
    ├── CMU.png
    └── NENU.png
```

## 如何使用
### `main.tex`
- 修改推荐信地址
    ```
    \hphantom{AA}Room xxx, Academic Building \\ % Change your address
    \hphantom{AA}School of Information Science and Technology \\
    \hphantom{AA}NorthEast Normal University \\
    \hphantom{AA}No.2555 Jingyue Street, Nanguan District \\
    \hphantom{AA}Changchun, P. R. China, 130117 \\
    ```

- 修改推荐信落款
    ```
    Sincerely yours,

    \includegraphics[width=2in]{pic/signature.png} % Please sign your name

    xxx, Professor \\ % Change your personal information
    School of Information Science and Technology \\
    NorthEast Normal University \\
    Phone: (86) 10-xxxx-xxx \\ 
    Email: \href{mailto:xxx@nenu.edu.cn}{xxx@nenu.edu.cn} \\
    Website: \url{https://ai.nenu.edu.cn} \\
    ```

- 修改推荐信 Logo
    ```
    pic/NENU_Logo_Bg.png % you may need to adjust the transparency of your picture.
    pic/NENU_Logo.png
    ```

### `letterContent.tex` 
> 此文件为推荐信的主内容
- 编辑你的内容
- 注意使用 `\\` 进行换行

## 如何编译
### 方式 1 ：在线编译
- 打开 [Overleaf](https://www.overleaf.com/latex/templates/nenu-letter-template/fvqdkcyhnbsv) 链接
- `Open as Template`
- 编辑你的内容
- 编译
- 下载 PDF

### 方式 2 ：本地编译
- 安装 Tex 本地环境: https://www.latex-project.org/get
- 下载此项目: `git clone https://github.com/leungll/NENU-Letter-Template.git`
- 运行: `pdflatex main`

## 参考
- [THU Letter of Recommendation Template](https://www.overleaf.com/latex/templates/thu-letter-of-recommendation-template/ghjfgfhykprk)
- [Learn LaTeX in 30 minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)

---
**This project needs a star ⭐ from you ❤️.**
