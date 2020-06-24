# LateX-Document

## Description : Study LateX by Visual Studio Code

### Deployment Environment：

#### 1. Install Visual Studio Code

Official Website: https://code.visualstudio.com/

#### 2. Install LateX 

Tsinghua Mirror : https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/

#### 3.Install Latex Workshop

Open Visual Studio Code and Open Setting "Ctrl +，"，paste the Configuration parameter , save the Configuration file.

```latex
"latex-workshop.latex.tools" : [
  {
      "name": "XeLaTeX",
      "command": "XeLaTeX",
      "args": [
          "-synctex=1",
          "-interaction=nonstopmode",
          "-file-line-error",
          "-pdf",
          "%DOCFILE%"
      ]
  },
  {
      "name": "pdflatex",
      "command": "pdflatex",
      "args": [
          "-synctex=1",
          "-interaction=nonstopmode",
          "-file-line-error",
          "%DOCFILE%"
      ]
  },
  {
      "name": "bibtex",
      "command": "bibtex",
      "args": [
          "%DOCFILE%"
      ]
  }
],
```

#### 4. Create New File 

Create the New File , such as *.tex . 

#### 5.Add Path

Add "%SystemRoot%\system32" to Environment variables Key Value

#### 6.Build Project

Use Hotkey , Ctrl + Alt + B  \ Ctrl + S

#### 7.Preview PDF files

After successful compilation, You can see the form at preview in the PDF file. The PDF Files on the Right Window.

### Key Point Word

