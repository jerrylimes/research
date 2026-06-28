# Editorial Notes

Notes I made as I'm going through the errata. Unfortunately this didn't occur to me when I was editing everything in I-1 so ...

Claude gave me a real banger the other day. "Original text can contain clues, issue description cannot add new clues."

## Errata in I-2

### 5483

The author of the original RFC, RFC 8846 included a fix that is different from the proposed fix in the Notes section of the report. There's no way I can make the model get to what the Notes is proposing because no reference was provided as to how the author reached that proposed fix.

### 5489

The last sentence of the original Explanation is kept. If the model figured out the fix too easily, that sentence should be deleted.

### 5845

The notes contain important information - so important I hated to remove them but I had to. Here are the Notes.
```
Description of whether Intermediate-Result TLV is supposed to be used in the case where only a single inner EAP authentication method is used. Section 3.3.1 says "more than one method is going to be executed in the tunnel, then upon method completion, the server MUST send an Intermediate-Result TLV indicating the result", Section 3.3.3 says "The Crypto-Binding TLV and Intermediate-Result TLV MUST be included to perform cryptographic binding after each successful EAP method in a sequence of one or more EAP methods", 4.2.13 says "It MUST be included with the Intermediate-Result TLV to perform cryptographic binding after each successful EAP method in a sequence of EAP methods", Annex C.3 shows an example exchange with a single inner EAP authentication method with use of Intermediate-Result TLV.


It looks like the majority of the places discussion this topic implies that there is going to be an Intermediate-Result TLV after each inner EAP authentication method and the text in 3.3.1 is the only clear case of conflicting (or well, at least misleading if one were to claim it does not explicitly say MUST NOT for the one inner EAP authentication method case). As such, I'd conclude the Intermediate-Result TLV is indeed going to be exchanged after each EAP authentication method and the proposed text change to 3.3.1 covers that.
```
If the model is not producing the correct fix we'd know what to do given this.

### 5945

is extremely long so good luck LLM.

### 7780

contains an incorrect Explanation. Nowhere in the "It should say" and "Notes" section did it say that **both** the client and the server must treat the GOAWAY frame as sth. It's either the client or the endpoint.

## Errata in U-1

### 4439

I hope the model knows how to find the `parameter` rule from RFC 7231 as a replacement because I sure as hell can't.

## Errata in U-2

## 5638

What counts as an under-specification and what counts as an inconsistency? This one really feels like an inconsistency to me.

## Errata in U-4

### 4413, 4509, and 6263

**HAVE** to be inconsistencies... the only things that were wrong are the section numbers and section names...

### 7866 

literally says "it is classified as INCONSISTENT" and it's under the under-specification folder.
