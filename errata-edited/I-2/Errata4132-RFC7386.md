# Errata 4132 - RFC 7386

- **RFC Title:** JSON Merge Patch
- **RFC Publication Date:** October 2014

```
Section 2 says:


define MergePatch(Target, Patch):

       if Patch is an Object:

         if Target is not an Object:

       Target = {} # Ignore the contents and set it to an empty Object

         for each Name/Value pair in Patch:

       if Value is null:

         if Name exists in Target:

           remove the Name/Value pair from Target

       else:

         Target[Name] = MergePatch(Target[Name], Value)

         return Target

       else:

         return Patch

// state how to fix the above text here

```

## Issue description

The indentation of the pseudocode example of Section 2 is incorrect. The erroneous indentation affects the interpretation of the conditional statements, leading to an incorrect merge algorithm and thus impacting the implementation of JSON Merge Patch.
