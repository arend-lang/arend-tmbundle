# Syntax highlighting for Arend

This repository contains (rudimentary) syntax highlighting for Arend

## For GitHub

To make a change to this grammar:
- change `Arend.yml` accordingly (see the [documentation of the grammar format](https://macromates.com/manual/en/language_grammars)),
- test your changes on [Lightshow](https://github-lightshow.herokuapp.com),
- generate the `Arend.tmLanguage` file using [this script](https://github.com/asciidoctor/sublimetext-asciidoc/blob/master/script/yaml-to-plist),
- commit and push your changes (or send a pull request to this repository),
- wait patiently for the next release and deployment of linguist on GitHub, the changes here will be taken into account automatically.

## For Sublime Text and bat

The command line tool [bat](https://github.com/sharkdp/bat) and [Sublime Text](https://www.sublimetext.com)
can use `Arend.sublime-syntax` to syntax highlight Arend.

To use it in bat:

```bash
mkdir -p "$(bat --config-dir)/syntaxes"
cd "$(bat --config-dir)/syntaxes"

git clone https://github.com/arend-lang/arend-tmbundle
bat cache --build
```
