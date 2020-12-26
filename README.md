# BNF
An expression tree is built using recursive descent which scans expressions that adhere the following BNF:

expression ::= factor * expression | factor / expression | factor
factor :== term + factor | term - factor | term
term ::= (expression) | literal
literal ::= 0|1|2|3|4|5|6|7|8|9

The tree is printed using Euler tour traversal. An integer valued function is written to scan the tree to evaluate the expression represented by the tree.
