# Syntax Highlighter for Google Sheets formulas

Syntax Highlighting for Google Sheets formulas in Visual Studio Code.

## Features

Syntax Highlighting for:
- Sheets Functions Keywords like `IF`, `DATE`, `DEC2HEX`, etc.
- Single line comments
- Double line comments
- Single quote strings
- Double quote strings
- Support for number highlighting
- Special Characters like `=`, `<>` , and `=!`

## Technical Information

Syntax highlighting is done by corresponding to textmate elements.

### Keywords

Patterns matched to `keyword.control`:
- `AND`
- `IF`
- `IFERROR`
- `IFNA`
- `IFs`
- `NOT`
- `OR`
- `SWITCH`
- `XOR`

### Comments

Pattern matched to `comment.line.double-slash`:

> lines starting with `//`

Pattern matched to `comment.block`:

> Blocks starting with `/*` and ending with `*/`

### Support

Patterns matched to `support.function`:

Every function listed in [Google's documentation](https://support.google.com/docs/table/25273?hl=en#).

### Strings

Pattern matched to `string.quoted.single`:

> Comments encapsulated by ' & '

Pattern matched to `string.quoted.double`:

> Comments encapsulated by " & "

### Constants

Pattern matched to `constant.character`:

> <,>,=,!,$,:

Pattern matched to `constant.language`:

> FALSE, TRUE

Pattern matched to `constant.numeric`:

> Numbers 0-9
