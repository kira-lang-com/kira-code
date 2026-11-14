# KiraCode

KiraCode is the code intelligence an editor asks for, in Kira: syntax
tokens, diagnostics, document structure, locations, completions and edits.
It answers in tokens, ranges and edits; colors, fonts and widgets belong to
the editor, and nothing here imports a UI module.

Every question goes through a `CodeSession`. Whoever answers it, the built-in
lexical grammars today, language servers and tree-sitter grammars behind
them, is an implementation detail the session hides: an editor asks the same
way whoever answers.

| Directory | What it holds |
| --- | --- |
| `app/Session` | `CodeSession`, its requests, answers and events |
| `app/Text` | `TextDocument` and positions |
| `app/Syntax` | Tokens, lexical grammars, the lexer and the highlighter |
| `app/Languages` | Language descriptions and the standard set |
| `app/Intelligence` | Diagnostics, structure, locations, assistance and edits |
| `app/Servers` | Language servers |
| `app/Storage` | Text storage |

## Use it

Add KiraCode to a package's dependencies in `package.kira`, then:

```sh
kira build
kira test
```

`RELEASE.md` holds the current week's notes. KiraCode is developed in the
Tessera monorepo and mirrored here by Cairn.
