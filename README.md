# tree-sitter-marte

[MARTe2](https://vcis.f4e.europa.eu/marte2-docs/master/html/) configuration file grammar for [tree-sitter](https://github.com/tree-sitter/tree-sitter)

## Usage
The parser can be used as a syntax highlighter by any editor using tree-sitter, like [neovim](https://neovim.io/), or in VScode with the [tree-siter-vscode](https://marketplace.visualstudio.com/items?itemName=AlecGhost.tree-sitter-vscode) extension.

The release provides the repository source code and a zip file containing the *.wasm* and *.scm* files needed by the editors to implement the syntax highlighting.

## Syntax
The [grammar.json](./src/grammar.json) file contains the grammar rules of the MARTe2 configurations files. The following list shows the main keywoard specifically  highlighted by the parser:
- *Class*, *DataSource*, *InputSignals*, *Type*, *NumberOfDimensions*, *NumberOfElements*
- The application name, identified by the initial character *$*
- The object names, identified by the initial character *+*
- MARTe2 types
- Strings
- Numbers
- Comments

## Example
![Alt text](./images/example.png "MARTe2 configuration file highligthing example.")

## ToDo
Add specific highlitghting rules for [MARTe2-components](https://github.com/aneto0/MARTe2-components).

## References
- [tree-sitter](https://tree-sitter.github.io)
- [MARTe2](https://github.com/aneto0/MARTe2)
- [MARTe2-components](https://github.com/aneto0/MARTe2-components)
- [MARTe2 documentation](https://vcis.f4e.europa.eu/marte2-docs/master/html/)
