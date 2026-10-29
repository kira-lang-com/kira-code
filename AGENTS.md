DO NOT create any "smoke test", "probe" and anything that isn't meant to either: showcase KiraCode or be driven by a real human. Anything called "smoke" or "probe" is outright **banned** from this repo.

This library has to be idiomatic, flawless, beautiful to read, kira native, using Kira's first party syntax. A single abstraction of the wrong shape, one stray helper, or one bad design and we FAILED.

KiraCode knows nothing about how an editor draws. It answers in tokens, ranges and edits; colors, fonts and widgets belong to the editor. Nothing here imports a UI module.

Every question an editor asks goes through `CodeSession`. A provider -- the built-in lexical grammars today, language servers and tree-sitter grammars behind them -- is an implementation detail the session hides: an editor asks the same way whoever answers.
