# Errata 4916 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016

```
Section 7.17. says:


If the target node is a container, list, case, input, output, or

notification node, the "container", "leaf", "list", "leaf-list",

"uses", and "choice" statements can be used within the "augment"

statement.

// state how to fix the above text here

```

## Issue description

The original text is missing two valid substatements from the list of allowed substatements within an "augment" statement when the target node is a container.
