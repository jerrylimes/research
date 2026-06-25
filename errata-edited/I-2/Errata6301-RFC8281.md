# Errata 6301 - RFC 8281

- **RFC Title:** Path Computation Element Communication Protocol (PCEP) Extensions for PCE-Initiated LSP Setup in a Stateful PCE Model
- **RFC Publication Date:** December 2017

```
Section 5.1 says:


     <PCE-initiated-lsp-request> ::= (<PCE-initiated-lsp-instantiation>|

                                      <PCE-initiated-lsp-deletion>)



     <PCE-initiated-lsp-instantiation> ::= <SRP>

                                           <LSP>

                                           [<END-POINTS>]

                                           <ERO>

                                           [<attribute-list>]



     <PCE-initiated-lsp-deletion> ::= <SRP>

                                      <LSP>

// state how to fix the above text here

```

## Issue description

The original specification is ambiguous about the scope of `<PCE-initiated-lsp-deletion>` requests.
