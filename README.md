# USST-OECE-ExpReport
This is a LaTeX template for University of Shanghai of Science and Technology, Optical Electronic and Computer Engineering Institute, experimentation reports.

上海理工大学光电信息与计算机工程学院实验报告的 LaTeX 模板。

###编辑：
一般情况下，无需修改 exp.tex, element/ExpHead.tex。
修改封面信息以及添加文件只需要在 contents.tex 中修改即可。其他可定制信息在 contents.tex 中已以注释方式说明。
建议编辑方式：每个实验使用单独的文件存放（exp/exp1.tex, exp/exp2.tex），在 contents.tex 中以 `\input{exp/exp?}` 的方式连接；文件按分类存放：
```
element - 模板中的固定文件，一般是科目无关的
exp     - 实验报告源文件
figure  - 图片（eps,png,jpg 均可）
listing - 清单（代码）
tabls   - 表格
tikz    - 使用 tikz 绘图的 tex 文件
```

###编译：
在根目录下使用 `xelatex exp` 即可编译，注意当使用 `minted` 宏包插入清单时请使用 `xelatex -shell-escape exp` 进行编译。 

###截图:
![PDF Preview](element/Preview-coverpage.png "Preview - Cover Page")
