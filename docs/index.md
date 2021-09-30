# Technical Documentation definition

*Technical Documentation means designs, reports, photographs, drawings, plans, specifications, computer software, surveys, calculations and other data, information and material collected, computed, drawn or produced, including computer print-outs;

## Tools available in Technical documentation 

* Adobe FrameMaker.
* Adobe RoboHelp.
* Text Editor for HTML.
* WordPress.
* Microsoft Visio.
* Windows Snipping Tool*

## The different themes in Mkdocs

* Creating a custom theme: The bare minimum required for a custom theme is a main.html Jinja2 template file which is placed in a directory that is not a child of the docs_dir. 

mkdocs.yml
docs/
    index.md
    about.md
custom_theme/
    main.html
    ...

* Basic theme: The body content from each page specified in mkdocs.yml is inserted using the {{ page.content }} tag. Style-sheets and scripts can be brought into this theme as with a normal HTML file. 

* Theme Files: There are various files which a theme treats special in some way. Any other files are simply copied from the theme directory to the same path in the site_dir when the site it built.

* Template Files: Any files with the .html extension are considered to be template files and are not copied from the theme directory or any subdirectories. 

* Theme Meta Files: The various files required for packaging a theme are also ignored. Specifically, the mkdocs_theme.yml configuration file and any Python files.



## Mkdocs syntax

* ```py
import this
print("Please document syntax highlighting in mkdocs")
```



<!-- 
# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files. -->
