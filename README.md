# Vim PlantUML Syntax/Plugin/FTDetect

This is [a fork repository by @rhysd](https://github.com/rhysd/plantuml-syntax)
([original repository](https://github.com/aklt/plantuml-syntax)).

This is a vim syntax file for [PlantUML](http://plantuml.com).

The `filetype` will be set to `plantuml` for *.pu, *.uml or *.plantuml files or if the
first line of a file contains `@startuml`.

Additionally the `makeprg` is set to `plantuml` assuming you have this
executable in your path.  This file could contain something like

````sh
#!/bin/bash
java -jar $HOME/lib/java/plantuml.jar -tsvg $@
````

You can change the name of this file by setting `g:plantuml_executable_script`
