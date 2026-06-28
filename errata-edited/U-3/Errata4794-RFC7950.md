# Errata 4794 - RFC 7950

- **RFC Title:** The YANG 1.1 Data Modeling Language
- **RFC Publication Date:** August 2016

```
Section 7.21.5 says:


   o  If the "when" statement is a child of an "augment" statement, then

      the context node is the augment's target node in the data tree, if

      the target node is a data node.  Otherwise, the context node is

      the closest ancestor node to the target node that is also a data

      node.  If no such node exists, the context node is the root node.

      The accessible tree is tentatively altered during the processing

      of the XPath expression by removing all instances (if any) of the

      nodes added by the "augment" statement.

// state how to fix the above text here

```

## Issue description

The original description of context node selection for "when" statements within "augment" statements incorrectly limits the context node to only data nodes, which is inconsistent with the definition of the accessible tree in Section 6.4.1.

**For this example, the correct fix has been provided to you as a guide to how to correctly disambiguate the erroneous text.**

## Correct fix

```
It should say:

   o  If the "when" statement is a child of an "augment" statement, then

      the context node is the augment's target node in the data tree, if

      the target node is a data node, rpc, action or notification.

      Otherwise, the context node is the closest ancestor node to the

      target node that is also a data node, rpc, action or notification.

      If no such node exists, the context node is the root node. The

      accessible tree is tentatively altered during the processing of

      the XPath expression by removing all instances (if any) of the

      nodes added by the "augment" statement.

```
