# Errata 5055 - RFC 7162

- **RFC Title:** IMAP Extensions: Quick Flag Changes Resynchronization (CONDSTORE) and Quick Mailbox Resynchronization (QRESYNC)
- **RFC Publication Date:** May 2014

```
Section 3.1.2.1 says:


   C: A142 SELECT INBOX

   S: * 172 EXISTS

   S: * 1 RECENT

   S: * OK [UNSEEN 12] Message 12 is first unseen

   S: * OK [UIDVALIDITY 3857529045] UIDs valid

   S: * OK [UIDNEXT 4392] Predicted next UID

   S: * FLAGS (\Answered \Flagged \Deleted \Seen \Draft)

   S: * OK [PERMANENTFLAGS (\Deleted \Seen \*)] Limited

   S: * OK [HIGHESTMODSEQ 715194045007]

   S: A142 OK [READ-WRITE] SELECT completed

// state how to fix the above text here

```

## Issue description

Section 3.1.2.1 presents a contradiction between the format of the HIGHESTMODSEQ response code and the requirements of RFC 3501. This inconsistency could result in implementations rejecting valid responses or producing invalid ones, thus directly affecting interoperability.
