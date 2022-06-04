## Lexical Analysis
---
- First phase of a compiler
- The lexical analyzer - reads stream of characters(source program) - groups the characters into meaningful sequences called lexemes.
- For each lexeme, lexical analyzer produces a $tokens$ of the form$$
<token-name, attribute-value>
$$

### Role
The main task of the lexical analyzer is to read the input characters of the source program, group them into lexemes, and produce as output a sequence of tokens for each lexeme in the source program.


### Tokens, Patterns, and Lexemes
- A token is a pair consisting of a token name and an optional attribute value. The token name is an abstract symbol representing a kind of lexical unit. $$
<token-name, attribute-value>
$$
- A pattern is a description of the form that the lexemes of a token may take.
- A lexeme is a sequence of characters in the source program that matches the pattern for a token and is identified by the lexical analyzer as an instance of that token.

### Specification Of Tokens
Regular Expressions are an important notation for specifying lexeme pattern.

#### Regular Expression

##### Regular Definition

###### Identifiers
$letter$_ -> $A | B | ... | Z | a | b | ... | z$
$digit$ -> $0 | 1 | 2 | ... |9$
$id$ -> $letter$_($letter$_|$digit$)$^*$

###### Unsigned Numbers
$digit$ -> $0 | 1 | 2 | ... |9$
$digits$ -> $digit\ digit^*$
$optionalFraction$ -> $.digits | \epsilon$
$optionalExponent$ -> $(E(+ | - | \epsilon)digits) | \epsilon$
$number$ -> $digits\ optionalFraction\ optionalExponent$





