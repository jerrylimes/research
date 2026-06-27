# Claude-suggested edits under I-1

Here is the conversation history between me and Claude on Jun 27, 2026 when I asked it to go over everything under the I-1 folder because I got scared by my stupidity.

### I said:

Can you go through all the errata reports in I-1 (/Volumes/Jerry/Source/Research/errata-edited/I-1) and

1. read the report
2. find if the issue description is not accurate. If there's a mistake, tell me, don't fix it yourself yet

### Claude:

119 files — I'll use an agent to go through them all systematically rather than doing it piecemeal.You are auditing errata report files that are being prepared as LLM training data. The goal is to train a model to detect errors in RFC specifications and produce a fix — WITHOUT being told the answer in the training data.

Each edited file (in `/Volumes/Jerry/Source/Research/errata-edited/I-1/`) has this structure:

- A "Section X says:" code block containing the original RFC text, followed by `// state how to fix the above text here` as a placeholder (replacing the original "It should say" block)
- An `## Issue description` section describing what's wrong

Each original file (in `/Volumes/Jerry/Source/Research/errata-original/I-1/`) has the full errata including the "It should say" block, Notes, and an `## Explanation` section.

**Your task**: Read EVERY edited file in `/Volumes/Jerry/Source/Research/errata-edited/I-1/`. For each one, also read the corresponding original. Then check the issue description for TWO things:

1. **Factual accuracy**: Does the issue description accurately describe the actual error shown in the original errata? If it says something wrong or misleading about what the error is, flag it.

2. **Too revealing**: Does the issue description give away the fix too directly? The test: could only one correction satisfy this description? If yes, it's too revealing. Describing the error _type_ (e.g., "incorrect type value", "missing field") is fine; naming the _correct value_ or _exact fix_ is not.

**What NOT to flag**:

- Descriptions that are vague or brief — that's fine and intentional
- Descriptions that reference terms already visible in the "Section X says" block
- Minor wording style issues
- Missing errata links (known issue, not relevant here)

**What TO flag**:

- Descriptions that are factually wrong about what the error is
- Descriptions that name the specific correct value, correct field, or exact fix
- Descriptions that are so narrow only one answer satisfies them (and it's the known fix)

Go through ALL 119 files. For each problem you find, report:

- Filename
- The problematic sentence(s) in the issue description
- Why it's a problem (inaccurate / too revealing)

If a file is fine, don't mention it. Produce a concise list of only the problematic files.

Let me spot-check a few of the agent's findings before reporting them to you.

Read 9 files

Read 9 files

### Here's the confirmed list of issues:

#### "It should say" block was not replaced — fix is fully visible:

* Errata8132-RFC9656.md — The entire corrected JSON with example: namespace prefixes is still present after "It should say:" on line 562. The fix is completely revealed.
* Errata6656-RFC8588.md — "It should say" block still present showing "iat":1443208345 (unquoted). Notes also still present.
* Errata4503-RFC7483.md — Partial: the Section 5.2 corrected entry ("unicodeName" : "ns1.fóo.example") is still there, with the placeholder only replacing the remaining Section 5.3 fixes. Notes also still present.

#### Structural issues:

* Errata4825-RFC7230.md — Header is still ## Explanation, not ## Issue description. Notes section is still present (the ICAP 0; ieof example). The description also says "The proposed change to include optional whitespace…" which directly names the fix.

#### Factually inaccurate descriptions:

* Errata7400-RFC8650.md — "according to RFC9112's CRLF requirement" is wrong. The trailing comma in Figure 16 is a JSON syntax error — nothing to do with CRLF or RFC 9112.
* Errata5021-RFC7788.md — "Section 9's definition of the DNCP_NODE_IDENTIFIER_LENGTH field" doesn't say which RFC's Section 9. The contradiction is with RFC 7787's Section 9, not RFC 7788's.

#### Too revealing:

* Errata5342-RFC83.md — "RP_Keepalive_Period, which may be shorter than the actual keepalive period" implies the fix is to use the maximum of the two periods. With only two named keepalive values in context, this points to a single answer.

#### Minor / debatable:

* Errata4935-RFC8080.md — "The four examples are not correctly identifying algorithms" is slightly imprecise. The algorithm field is only wrong in the RRSIG records specifically — the DNSKEY and DS records are fine. "Four examples" is ambiguous about what it refers to.
