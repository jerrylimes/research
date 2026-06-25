# Errata 5877 - RFC 8579

- **RFC Title:** Sieve Email Filtering: Delivering to Special-Use Mailboxes
- **RFC Publication Date:** May 2019

```
Section 6 says:


require "imapsieve";

require "special-use";

require "environment";

require "variables";



if environment :contains "imap.mailbox" "*" {

    set "mailbox" "${1}";

}



if allof(

    environment "imap.cause" "COPY",

    specialuse_exists "${mailbox}" "\\Junk") {

    redirect "spam-report@example.org";

}

// state how to fix the above text here

```

## Explanation

The original example uses an incorrect match type for extracting a match variable. This inconsistency would affect the operation of the Sieve script.
