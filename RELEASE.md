# 26.10.4

**Project:** KiraCode  
**Release week:** 2026-10-26 – 2026-11-01

## Highlights

The first source release of KiraCode provides `CodeSession` for editor-facing tokens, ranges, and edits. It includes built-in lexical grammars and keeps syntax providers separate from editor drawing, colors, fonts, and widgets.

## Changed

- Updated `CodeSession` to mark unchecked native interop operations with explicit Kira unsafe scopes.
