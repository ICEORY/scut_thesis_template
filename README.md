## 华南理工-学术型硕士-毕业设计-latex-模板

---

### 资料来源：http://www.latexstudio.net/archives/6222

### 说明：

看了一下华工的硕士的毕业设计模板要求跟博士的是一样的，所以直接使用博士的学位论文。稍微改了一下名称而已。感谢作者 **徐川页** 的工作

### 如何使用：

1. 编译：使用xelatex进行编译（支持中文）， texsudio 设置：options --> configure --> build --> default compiler --> select xelatex 

2. 提名页直接在 thesis_cover.docx 中进行修改，然后导出为pdf，覆盖原来的 thesis_cover.pdf 文件即可

3. 论文的模板定义在 scutthesis.cls 中进行修改，如果看不懂怎么修改的话，最好不要动这个文件。

4. 个别细节的调整：超链接的颜色或者引用的颜色，在scutthesis.tex 内容的开头 \hypersetup 中进行自定义

   ```latex
   \hypersetup{pdftitle={学术型硕士论文标题},
    pdfauthor={你的名字},
    pdfsubject={华南理工大学学术型硕士学位论文},
    pdfkeywords={关键字1, 关键字2},
    unicode=false,linkcolor=black, anchorcolor=black, citecolor=olive, filecolor=magenta, menucolor=red, urlcolor=magenta, pdfstartview=FitH}
   ```

5. 参考文件的格式在 scutthesis.bst 中定义

6. 添加参考文献在 reference.bib 中进行修改