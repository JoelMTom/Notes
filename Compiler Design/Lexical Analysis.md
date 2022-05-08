#### Lexical Analysis
---
##### Role
The main task of the lexical analyzer is to read the input characters of the source program, group them into lexemes, and produce as output a sequence of tokens for each lexeme in the source program.


#### Tokens, Patterns, and Lexemes
- A token is a pair consisting of a token name and an optional attribute value. The token name is an abstract symbol representing a kind of lexical unit.
- A pattern is a description of the form that the lexemes of a token may take.
- A lexeme is a sequence of characters in the source program that matches the pattern for a token and is identified by the lexical analyzer as an instance of that token.

#### Specification Of Tokens
Regular Expressions are an important notation for specifying lexeme pattern.

