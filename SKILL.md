---
name: ste100
description: Apply ASD-STE100 Simplified Technical English Issue 9 principles to technical and business text. Use when the user asks to write, rewrite, simplify, convert, review, check, audit, or improve text for STE/STE100/Simplified Technical English, including emails, RFIs, reports, procedures, instructions, site notes, specifications, commissioning text, safety text, and construction documentation. Support both rewrite-only and compliance-review modes. Treat established construction and electrical terminology as permitted technical nouns or technical verbs when used with their standard industry meaning, unless the user asks for stricter dictionary-only treatment.
---

# STE100

Apply ASD-STE100 Issue 9 principles while preserving the user's technical meaning, responsibilities, quantities, references, and contractual intent.

## Workflow

1. Identify the requested mode.
   - If the user says **rewrite**, **convert**, **make this STE**, **simplify**, or equivalent: return the rewritten text only, unless a short note is necessary to explain an unavoidable ambiguity.
   - If the user says **check**, **review**, **audit**, **compliance**, **what is wrong**, or equivalent: perform a compliance review and then provide a corrected STE version.
   - If the request is ambiguous, use rewrite mode and do not burden the user with a full audit.
2. Identify the text type before editing: procedural, descriptive, safety instruction, or mixed.
3. Preserve technical facts and source meaning. Do not invent missing design information, responsibilities, approvals, causes, dates, quantities, or commitments.
4. Apply the rules in `references/core-rules.md`.
5. Apply the construction terminology policy in `references/construction-terminology.md`.
6. For review mode, use the output pattern in `references/review-output.md`.
7. Do a final verification pass for sentence length, voice, terminology consistency, word meaning, and technical fidelity.

## Scope

Apply the skill to all user-provided text types unless the user excludes a type or asks for a different style. This includes correspondence and construction-management documents, even though STE was developed for technical documentation.

Do not force a procedural style onto correspondence. Classify normal emails, RFIs, reports, narratives, explanations, and scope descriptions as descriptive writing unless they contain direct work instructions.

## Technical fidelity

Preserve exactly when present:
- equipment and system names
- drawing, specification, RFI, SI, CO, change, and document references
- model numbers, part numbers, circuit numbers, panel names, tags, room names, and identifiers
- dimensions, units, voltages, ratings, quantities, dates, and times
- code, standard, contract, and clause references
- proper nouns, company names, project names, and quoted text
- established abbreviations and acronyms, unless the user asks to expand them

Do not replace a technical term merely because it is not ordinary STE vocabulary when it qualifies as an established technical noun or technical verb.

## Meaning before form

Never make a word-for-word replacement that changes the technical or contractual meaning. If a direct replacement is not accurate, rewrite the sentence construction.

When source text is ambiguous, do not silently choose a meaning. Preserve the ambiguity if necessary and identify it in review mode. In rewrite-only mode, ask a question only when an accurate rewrite is not possible without clarification.

## Compliance claims

Do not claim formal ASD certification or guaranteed full dictionary compliance. Say "STE-style", "aligned with ASD-STE100 Issue 9", or "reviewed against the available Issue 9 rules" when a qualification is necessary.

The bundled references are a working summary, not a reproduction of the full ASD dictionary. If exact status, approved meaning, or part of speech of an unusual non-construction word is uncertain, mark it for dictionary verification instead of inventing an answer.
