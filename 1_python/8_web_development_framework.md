# Web Development Framework

| FramEwork | Architecture                                              | html extensions | path for html                              | template engine                 |
| --------- | --------------------------------------------------------- | --------------- | ------------------------------------------ | ------------------------------- |
| Bottle    | MICRO (less configuration, mostly used for small web app) | .tpl            | TEMPLATE_PATH(append html file path to it) | Simple template engine, its own |
| FLASK     | MICRO                                                     | .html           | create dir template and add all .html      | JINJA2                          |
| Django    | MVT (highly configurable)                                 | .html           | same as flask                              | Django template engine          |
| Pyramid   | MVC  (medium)                                             |                 |                                            |                                 |
| web2py    | MVC                                                       |                 |                                            |                                 |

- All framework comes with any **WSGI** [Web Server Gateway Interface]() compatible **Server**.
- We can write python inside html files.
- python code interpretation is taken care by `template engine`



| title          | bottle       | flask         | django        |
| -------------- | ------------ | ------------- | ------------- |
| Python Tag     | %statement   | {%statement%} | {%%statement} |
| variable value | {{var_name}} | {{var_name}}  | {{var_name}}  |
|                | %for         | {%for%}       | {%for}        |
|                | %end         | {%end for%}   | {%end for%}   |
|                |              |               |               |



#### Webservices:

- Suppose we have PVR website, and BookMyShow website, PVR needs to share its data to BookMYshow.

- To achieve above condition PVR has to expose one API which will share data and BookMyShow will call that API.

- To Create these we API `Application Programming Interface`, we can use below protocols - 

  - [SOAP]() ` Simple Object Access Protocol` : 
    1. It has its own protocol, so complex to use.

  - [REST]() `Representational State Transfer`
1. It uses http protocol only, simple to use.





