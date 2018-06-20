# LaTex环境搭建
## sublime text 3 + Miktex 
- 安装Sublime Text 3，经典安装
- 安装Miktex，经典安装，自动添加环境变量
- 安装Sublime插件，Latextools
- 安装SumatraPdf
- 设置从pdf跳转回tex代码处：SumatraPDF.exe -inverse-search"\\"SUBLIME_PATH" \\"%f:%l\\"" (测试无效，不管了)
- ok
- ctrl+b: build; 双击SumatraPdf跳转至相应代码处。
## vs code + Miktex ##
- 安装vs code
- 安装Miktex
- 安装vs code插件：LaTeX workshop
- 配置LaTeX workshop设置："latex-workshop.latex.recipes": [{
  "name": "texify",
  "tools": [
    "texify"
  ]
}],
"latex-workshop.latex.tools": [{
  "name": "texify",
  "command": "texify",
  "args": [
    "--synctex",
    "--pdf",
    "--tex-option=\"-interaction=nonstopmode\"",
    "--tex-option=\"-file-line-error\"",
    "%DOC%.tex"
  ]
}]
