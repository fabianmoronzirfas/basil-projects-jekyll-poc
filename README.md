Basil.js Projects with Jekyll
=============================

This is a proof of concept for creating a simple structure where users can submit projects that can be parsed with Jekyll.  

## Structure

The folder and file structure for a project should be as simple as possible. It could be like this:  

    projects/example/
    ├── images
    │   ├── boom.png
    │   ├── canvas.png
    │   └── foobah.png
    ├── index.js
    └── index.md

- The images folder can contain as many images as the user wants.
- The index.js contains the code for the project. It must be one file currently and it has to be named index.js
- The index.md contains a YAML header to discribe the project and some additional text if the user feels to write something about it.  

## YAML Header

This is the only point where errors might occur. If something is typed wrong it might produce errors. It ould be like this:  

    ---
    # The name for the layout to use
    # should always be project
    layout: project
    # The title for this project
    # needs to be in ""
    title: "This is my funky Basil.js project"
    # we could also add things like
    # authors: 
    #    - "Bugs Bunny"
    #    - "Duffy Duck"
    # Or even contact or URLs
    # The type. This is for identifying project pages
    type: project
    # All the images that are in the images folder that should be displayed
    images:
        - "boom.png"
        - "canvas.png"
        - "foobah.png"
    # A short summery of the project
    summary: "This is a short summary of my funky basil.js Project"
    ---

Of course the above yaml header has lots of comments. A boiled down version would look like this:  

    ---
    layout: project
    title: "This is my funky Basil.js project"
    type: project
    images:
        - "boom.png"
        - "canvas.png"
        - "foobah.png"
    summary: "This is a short summary of my funky basil.js Project"
    ---

To be continued (eventually)

## License

Copyright (c)  2017 Fabian Morón Zirfas  
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software  without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to  permit persons to whom the Software is furnished to do so, subject to the following conditions:  
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.  
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A  PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF  CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.  

see also http://www.opensource.org/licenses/mit-license.php

