# Py.Html Documentation 
### Framework for create web projects with python tecnology.

# Introducion to Py.Html
The **Py.html** is one framework write in python for web projects create.
  
Algorithm makes an HTML file from scratch starting idea is *organization* where for each document **HTML, CSS or JS**  stay with good write and functions .

**Development team:**
*Felipe Catão* - Fullstack developer

# Sumary: 
In this document your can see: 

**Part one: Basic functions**
-  How to use Py.html 
     +  About py.html
     + How to import Class 
     + WorkFlow Py.html
     
- Create Html code with Python
     + Basic Html  code
     + Don´t edit Html code dude!
     + Envirioment and path
     + Start Project
     
- Edit Html Code 
     + Now, edit Html code, with Py.html
     + Less code , more functions
     
 **Part two: Advanced modules**
- Create Css and Link to *Html*
     + Basic command to Html fol tag < link >
     + Create manual config *Css*
     + Suport guide to *Css and Js*
     
- Inside Modules : **HtmlPy()** and  **CssPy()**
     + The PyHtml.py Code 
     + The HtmlPy() Module 
     + The CssPy() Module
     + Index and vars 
     + Create multi function
- CssPy() Module
    + Basic Css rules 
    + ( Others functions )
    + Animate Basic functions 
    + Advanced Function Animate Css

#  Part one: Basic functions 
Hello, if your install the *Py.html* now, start to its in this block your learn to: create and edit code html and css with py.html tecnology, one note very important  **PyHtml is organization web project , not one creator and editor web.** Its tool  is very cool for start project with basic elements not one very big editor web, we use this note in mind.

## About py.html 
The py.html is on framework to create envirioment to web projects, but your project will complete with edition direct in HTML and CSS code. The Py.Html some create base to your code.

### How to import Class
The main class this framework is PyHtml.py, it create html,css and js code also edit and creater new components to your project, frist fime your download (or clone ) Py.html from [Github Py.html](https://github.com/FelipeKatao/Py.Html) to your path destiny, in future the resource install via pip stay avaliable.

Now in your code python start writer the frister line is: 
`from Framework import PyHtml`.
This line import to your python code the functions avaliable in PyHtml class start your code use the code:
```
from Framework import PyHtml

def main():
    html = PyHtml.htmlPy()
    html.CreateNewHtml("Home Page",R"Example\index.html",1)
    
```
In this code have 3 arguments basic its arguments create in your path destiny one Html code with or without coed base.

| Argument | Function |
|:--------:| -------------:|
| NameHtml | Define name your Html define some the title code no define name this file. |
| LocalFile|Destiny path your HTML code this argument have extension .html with name *ex: R"Example/code.html*
| PreCode | This argument should input 1 or 0 value, where 1(create Html code with  base) 0 (create html code some basics tags)

###    WorkFlow Py.html
Well we create basic code html with Py.Html was and now? Next step?
1. Create path with CSS and HTML code base.
2. Create HTML tags, after CSS code.
3. Create component Html 
4. Edit HTML and create rules to CSS files

In your Python code, your call function to creation Tags or Rules Css after create its your erase and create new tags or rules for tags in Htmlcode.
Thing  in your mind the code in python can static or dynamic your decide:

| Type Py code | Function |
|:--------:| -------------:|
| **Static** |In dynamic your not erases functions,some edit in HTML code, if your edit Py code not is one good pratical, some create new HTML or edit style from your project.
|**Dynamic**|In this model your create and erases new functions, always editing and new code from py code.

## Create Html code with Python
Now creater Html code using Py.html , preview we creater HTML base code was can create Html pré code with module PyHtml.py

### Basic Html  code
```
from Framework import PyHtml

def main():
    html = PyHtml.htmlPy()
    html.CreateNewHtml("Home Page",R"Example\index.html",1)
    
```
This basic code create Html code, now create tags to your Html. Stater create **Div** tag: 
```
html.createNewElement(R"Example\index.html","#NewDiv","div",10,"Helloworld"
```
This function create new element , not   necessarily need one **Div** tag can see img,h1,h2,span... Your decide type tag to be, how function parameters to *createNewElement* :

| Argument | Function |
|:--------:| -------------:|
| local |Destiny path your HTML code this argument have extension .html with name *ex: R"Example/code.html*
| id | what your Id from your element < tag >
| Element | What is element tag.
| LineIndex | What Line its element will be add in html file.
| Value | Value from element to your tag.

### Don´t edit Html code dude! 
In this stage not modify your code direct in Html, use Python code for its, only modify direct in Html after finish basic Html base code[^1]
Thing if your use Py.Html for create news tags use the Python code, for edit  this tags be use editing Html code.

### Envirioment and path
The envirioment your can  create variables to save and user in future in yours news functions, for use efficient use for envirioment you can use class **SearchData()**, the function is for save and analitic your code Html and content, in this moment we create envirioment and Path: 
```
from Framework import PyHtml

def main():
    html = PyHtml.htmlPy()
    data= PyHtml.SearchData()
    data.createNewFileLocal(R"Example\index.html","","")
    html.CreateNewHtml("Home Page",data._localHtmlFiles[0],1)
```
This function can create environment with files **HTML**,**CSS**,**JS** in we case crate path Html, the parameter aceppt the path or  void " ", if void the Py.html not create news path, the function respectively follow Html,Css and Js files.
### Start Project
With basic code , now start project!  From start the module PyHtml.py is much and very important for start project, go start with class HtmlPy()  is base from to initial project.

## Edit Html Code






[^1]:The Base code: Is your Html with structure ( head, body) good defined, navs, body this basic Html without Css.
<!--stackedit_data:
eyJkaXNjdXNzaW9ucyI6eyJlZ2xTY2Jsd3AyRkdmNGlSIjp7In
N0YXJ0IjoxODc0LCJlbmQiOjE5MTYsInRleHQiOiJUaGUgUHku
SHRtbCBzb21lIGNyZWF0ZSBiYXNlIHRvIHlvdXIgY29kZS4ifX
0sImNvbW1lbnRzIjp7InFOMEVJUjZaNUtrSmE0a08iOnsiZGlz
Y3Vzc2lvbklkIjoiZWdsU2NibHdwMkZHZjRpUiIsInN1YiI6Im
doOjM0NTU5MDgxIiwidGV4dCI6IkVzdGEgcGFydGUgZXN0YSBj
b20gIHVtYSBzaW50YXhlIHF1ZWJyYWRhLiIsImNyZWF0ZWQiOj
E1NTg1Nzk2MzQ5MTl9fSwiaGlzdG9yeSI6WzQ2MjkxNzUxMSwt
MTA1MjkxNDU4NSwtMTIzMjY5NTg0NCwxOTM5MTE5OTA2LDYzOD
k5Mjg1LC05NTQ0ODU4NzAsMTM4OTExNDAyMSwtMTc5NTE3ODY5
NCwtMzE1NTQ1Njg3LC03NDY2Mjc4MjYsMTM2ODU2MjQ3NywtOT
U1ODk4MDEyLDE1Nzk4ODE2MTIsMTA1NDM3MzY2NiwtMTQxNTY3
OTUzMywtMTk0MTI5NzA5NywtNzExNTg1NjM5XX0=
-->