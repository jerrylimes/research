# Errata 5807 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016

```
Section 7.21.5. says:


   o  If the "when" statement is a child of a "uses", "choice", or

      "case" statement, then the context node is the closest ancestor

      node to the node with the "when" statement that is also a data

      node.  If no such node exists, the context node is the root node.

      The accessible tree is tentatively altered during the processing

      of the XPath expression by removing all instances (if any) of the

      nodes added by the "uses", "choice", or "case" statement.

// state how to fix the above text here

```

## Explanation

The original description of context node selection for "when" statements within "uses", "choice", or "case" statements incorrectly limits the context node to only data nodes, which is inconsistent with the definition of the accessible tree in Section 6.4.1.
