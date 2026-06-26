# Errata 7058 - RFC 9132

- **RFC Title:** Distributed Denial-of-Service Open Threat Signaling (DOTS) Signal Channel Specification
- **RFC Publication Date:** September 2021

```
Section 5.3 says:


              uses data-channel:target {

                when "/dots-signal/scope/conflict-information/"

                   + "conflict-cause = 'overlapping-targets'";

              }

// state how to fix the above text here

```

## Issue description

The original YANG uses statement applies the augmentation to a scope that is larger than intended.  This creates an inconsistency between the intended behavior and the actual effect of the YANG statement.
