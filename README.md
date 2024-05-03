# Monkey

Following along with "Writing an interpreter in Go" book

## Lexer
Transformation from source code to tokens, is called “lexical analysis”, or “lexing” for short. It’s done by a lexer (also called tokenizer or scanner – some use one word or the other to denote subtle differences in behaviour).

## Tokens
Tokens are small, easily categorizable data structures that are then fed to the parser, e.g. `"let x = 5 + 5;"` might become:
```
[
  LET,
  IDENTIFIER("x"),
  EQUAL_SIGN,
  INTEGER(5),
  PLUS_SIGN,
  INTEGER(5),
  SEMICOLON
]
```

## Parser
Takes source code as input (either as text or tokens) and produce a data structure which represents this source code. The process of parsing is also called syntactic analysis.

## Additions not in book
1. Identifiers can have '?' characters in.

## Ideas for Further developments
1. p.15 - add support for Unicode (and emojis!).

