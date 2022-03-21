# VS-CODE-SETTING

## plugin

- Code Runner
  this plugin can run your code easily, and if you install this plugin, your right-top menu whill show a shape that like triangle, you chick this shape, vs code will according to your file suffix to use can run this language compiler or interpreter. so this plugin is important in your running.
- LaTex Workshop
  If you have texlive, use vs-code instead of texstudio, I think you will be intimidated by this plugin, it can show you some latex symbols, as well as code highlighting and code hinting, but I think it has one drawback of mine. AutoBuild, this plugin will rebuild if you change the tex file, you can stop it by setting.
- Markdown PDF
  Sometimes you want to convert markdown to pdf, you will use the browser to open makedown and save it as pdf, but in vscode, you only need a plug-in which is Markdown PDF, this plug-in can be saved as ".png", ".html", " pdf" ","jpeg", but if you use this plugin, you know that this plugin first makes makedown save as html, and second, it makes html save as pdf.
- Markdown Preview Enhanced
  This plugin can easily display the pdf made by markdown, which is very important in our use. You can see some modifications in this file.
- Extension Pack for Java
  include some plugin, such as
  - Language Support for Java(TM) by Red Hat,
  - Debugger for Java
    I think this plugin may be used in Debug, but I rarely use debug. Maybe I'm not a good programmer.
  - Test Runner for Java
  - Maven for Java
    Maven can manage packages
  - Project Manager for Java
  - Visual Studio IntelliCode
  - AI-assisted development
- python
  If you want write python file, maybe you need highlighting and code hinting, so you need this plugin,
- c/c++
  this plugin can provide highlighting and code hinting.
- Excel Viewer
  if you want to read Excel file, you should install this plugin, this plugin is just like its name.
- HTML Format
  sometime you want to write HTML, but you know formatting is problem, html syntax is complicated. this plugin can makes it easy.

# VS-CODE-USELOG

## language ##
if you want to used chinese, you should :
- install plugin which named "Chinese (Simplified) (简体中文) Language Pack for Visual Studio Code"
- used hotkey "Ctrl + shift + p"
- input "Dsiplay language"
- choose zh-cn or you alse can choose en

## setting snippets ##

* Ctrl+shift+p
* choice preferences: "configure user Snippets"
* you should input your language as file name.
  
```json
	 // Example:
	  "Print to console": {
	 	"scope": "javascript,typescript",
	 	"prefix": "log",
	 	"body": [
	 		"console.log('$1');",
	 		"$2"
	 	],
	 	"description": "Log output to console"
```

## markdown ##
- some Latex symbols
  you can used markdown to record some note, like math formula, and you want to used latex symbols, used like ”$ $“ can let vs-code show math formula. you can View, but if you want to print the pdf file, you should modify some setting file 
  ```shell
  sudo gedit ~/.vscode/extensions/yzane.markdown-pdf-1.4.4/template
  ```
  and you should input Ctrl + Shift + P and choice "> **Markdown Preview Enhanced: Run Code Chunk** " to source this setting file,  then , you can print to PDF

- Align left or Align right
  ```markdown
  <p align="right"> </p>
  ```

- remove header (some word in paper top)
  you need to find some setting in vs-code , you can search "Display Header Footer", and chick it. 
  
- markdown to print flow chart
  - like
    ```text
      ```mermaid
      graph TD;
    ```
  - some Attributes
    - TB	top to bottom
    - BT	bottom to top
    - RL	right to left
    - LR	left to right
  - some graphics setting
    - define is rectangle
    - the rectangle which border is circle
    ```markdown
    lab(word)
    ``` 
    - circle
    ```markdown
    lab((word))
    ```
    - diamond
    ```markdown
    lab{word}
    ```
    - Hexagon
    ```markdown
    lab{{word}}
    ```
    - Parallelogram
      - left to right
      ```markdown
	    lab[/word/]
      ```
      - right to left
      ```markdown
      lab[\word\]
      ```
    - some line
      - define is line which have arrow
      - only line
      ```markdown
      labA -- labB
      ```
      - point and point
      ```markdown
      labA -.- labB
      ```
      - bold line
      ```markdown
      labA ==> labB
## permissions errer

- **Insufficient permissions. Select 'Retry as Sudo' to retry as superuser.**
  This means you don't have enough permissions to save this file, you should check if this file was created by you, if you didn't create this file, you won't be able to change this file. And you can use like this:
  ```shell
  sudo chmod -R 777 [dir]
  ```
  This action allows other users to change the directory.

## python errer

- **nconsistent use of tabs and spaces in indentationPylance**
  Because you used spaces and tabs at the same times,but python don't allow you use simultaneously space and tabs,so you can use tab all the time or only use space, and you can click menu like View, then you can select Render Whitespace, this menu can render space and tabs, so you can easy to diffence them, and save this problem