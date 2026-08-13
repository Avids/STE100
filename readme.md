# STE100

A ChatGPT Skill for applying **ASD-STE100 Simplified Technical English (STE), Issue 9** principles to technical, construction, and business writing.

The skill is designed to make technical communication clearer, shorter, more consistent, and less ambiguous while preserving the original technical meaning, responsibilities, quantities, references, and contractual intent.

## What this Skill does

STE100 can write, rewrite, simplify, review, or audit text using ASD-STE100 Issue 9 principles.

It can be used with:

* Emails
* RFIs
* Technical reports
* Procedures
* Work instructions
* Site instructions
* Site notes
* Specifications
* Scope descriptions
* Commissioning documents
* Safety instructions
* Change-related correspondence
* Construction documentation
* General technical and business writing

The skill applies to all text types by default unless the user specifically excludes a type.

## Main operating modes

### Rewrite mode

Use this mode when you want cleaner STE-style text without a detailed explanation.

Example prompts:

```text
Rewrite this in STE100.
```

```text
Make this email STE100 compliant.
```

```text
Simplify this RFI using STE.
```

```text
Convert this procedure to Simplified Technical English.
```

The skill returns the rewritten text while preserving the technical meaning.

### Review mode

Use this mode when you want to identify problems and understand why changes are required.

Example prompts:

```text
Check this against STE100.
```

```text
Review this procedure for ASD-STE100 compliance.
```

```text
Audit this RFI using STE100.
```

```text
What STE100 issues are in this text?
```

The skill provides:

1. A concise compliance review.
2. Applicable STE rule references when available.
3. Recommended corrections.
4. A complete corrected version.

## Construction and electrical terminology

This skill is adapted for construction use.

Established construction terminology is treated as valid **technical terminology** when it has a recognized industry meaning.

The skill does not replace a technical term simply because the term is not part of ordinary STE vocabulary.

Examples of permitted technical terms include:

```text
conduit
raceway
cable tray
junction box
pull box
panelboard
switchboard
transformer
disconnect
breaker
feeder
branch circuit
fire alarm
annunciator
strobe
relay
rough-in
fit-out
energize
de-energize
terminate
firestop
commission
RFI
submittal
shop drawing
site instruction
change order
shutdown
outage
tie-in
```

These are examples only. Other established construction terms are also permitted when they have a recognized technical meaning.

The same principle applies to electrical, fire alarm, security, communications, controls, mechanical coordination, architectural, civil, commissioning, estimating, scheduling, contract administration, and site logistics terminology.

## Technical meaning takes priority

STE100 does not simplify text at the expense of technical accuracy.

The skill preserves, where applicable:

* Equipment and system names
* Drawing references
* Specification references
* RFI and site instruction numbers
* Change order references
* Model and part numbers
* Circuit numbers
* Panel names
* Equipment tags
* Room names
* Dimensions
* Units
* Voltages
* Ratings
* Quantities
* Dates
* Times
* Code references
* Standard references
* Contract clauses
* Company names
* Project names
* Established abbreviations
* Quoted text

If a direct word replacement changes the meaning, the skill changes the sentence structure instead.

## Construction responsibility and contractual language

STE100 is designed to avoid changing contractual or project-management meaning during editing.

It must not:

* Change a recommendation into a requirement.
* Change a target date into a guarantee.
* Transfer consultant responsibility to the contractor.
* Transfer owner responsibility to the contractor.
* Remove a prerequisite for performing work.
* Remove a schedule dependency.
* Remove a condition that protects contractual entitlement.

For example, language such as the following is preserved when it is necessary:

```text
subject to
contingent upon
after approval
after receipt of the site instruction
when access is available
upon receipt of the revised drawing
subject to material availability
```

The sentence can be simplified, but the dependency must remain.

## Key STE100 rules applied

The skill uses a working implementation of ASD-STE100 Issue 9 rules.

### Vocabulary

Use:

* Approved STE words.
* Technical nouns.
* Technical verbs.

Use an approved word only with its approved meaning and grammatical function.

Keep terminology consistent throughout the text.

### Multi-word technical nouns

Prefer technical nouns with no more than three words when practical.

For an official technical term longer than three words:

1. Write the complete term first.
2. Then use a clear shorter term or approved abbreviation when appropriate.

Do not shorten an official technical term if doing so could change its meaning.

### Verbs

Prefer simple verb forms.

Use active voice whenever practical.

For example:

```text
Passive:
The circuits are connected by the switching relay.

STE:
The switching relay connects the circuits.
```

For procedures, use direct commands:

```text
Non-STE:
The conduit is to be installed above the ceiling.

STE:
Install the conduit above the ceiling.
```

### Procedural writing

For procedures and work instructions:

* Maximum 20 words per sentence.
* Give one instruction per sentence unless actions occur at the same time.
* Use the imperative form.
* Put necessary conditions before the instruction.
* Do not place instructions or requirements inside notes.

Example:

```text
Before you energize the panel, complete the insulation-resistance test.
```

### Descriptive writing

For emails, RFIs, reports, explanations, scope descriptions, and similar text:

* Maximum 25 words per sentence.
* Give information gradually.
* Keep one main topic per paragraph.
* Use no more than six sentences in a paragraph.
* Keep terminology consistent.
* Prefer active voice.

### Safety instructions

Safety instructions must:

1. Identify the applicable risk category.
2. Give a clear command or condition.
3. Explain the hazard or possible result.

The skill does not invent safety classifications.

### Punctuation

STE100:

* Does not use semicolons.
* Uses vertical lists when they improve clarity.
* Uses hyphens only when words are directly related.
* Avoids unnecessary punctuation complexity.
* Checks sentence length using ASD-STE100 word-count principles.

## Example: construction email

### Original

```text
Please be advised that we are planning on proceeding with the installation of the conduit in the ceiling space on Monday, however this will be subject to receiving the revised lighting drawings and confirmation that the area has been made available for our work.
```

### STE100-style version

```text
We plan to install the conduit above the ceiling on Monday. This work is subject to receipt of the revised lighting drawings and available access.
```

The revised version is shorter, but it preserves the schedule dependencies.

## Example: RFI

### Original

```text
It has been noted that the electrical drawings do not appear to indicate where the fire alarm relay is intended to be located and therefore we are requesting that the consultant provide clarification regarding the required mounting location.
```

### STE100-style version

```text
The electrical drawings do not show the required location of the fire alarm relay. Please confirm the relay mounting location.
```

## Example: procedure

### Original

```text
Prior to commencing the installation of the feeder conductors, the electrician shall ensure that the conduit has been completely installed and that it is free from debris.
```

### STE100-style version

```text
Before you install the feeder conductors, make sure that the conduit is complete and free from debris.
```

## Example: compliance review

Prompt:

```text
Check this against STE100:

The contractor shall carry out testing of the system after the installation has been completed; thereafter the results should be forwarded to the consultant.
```

Typical review:

| Text / issue              | Rule area     | Finding                           | Correction                                |
| ------------------------- | ------------- | --------------------------------- | ----------------------------------------- |
| `shall carry out testing` | Words / verbs | Complex construction              | Use a direct verb construction            |
| Semicolon                 | 8.1           | Semicolons are not permitted      | Use separate sentences                    |
| `thereafter`              | Vocabulary    | Simplify the sequence             | Use `then` or another clear construction  |
| `should`                  | Meaning       | Could change requirement strength | Determine whether the action is mandatory |

Corrected version, if both actions are mandatory:

```text
The contractor must test the system after installation. Then, the contractor must send the test results to the consultant.
```

The skill does not automatically change `should` to `must` unless the source meaning shows that the requirement is mandatory.

## Recommended prompts

### Rewrite

```text
@STE100 Rewrite this email.
```

```text
@STE100 Rewrite this RFI using ASD-STE100.
```

```text
@STE100 Simplify this technical report.
```

### Review

```text
@STE100 Check this for STE100 compliance.
```

```text
@STE100 Review this procedure and show the rule violations.
```

```text
@STE100 Audit this construction specification using STE100.
```

### Restrict the scope

```text
@STE100 Review the procedure only. Do not change the email introduction.
```

```text
@STE100 Improve sentence structure only. Keep all construction terminology unchanged.
```

```text
@STE100 Use stricter dictionary-only STE treatment.
```

## Important limitations

This skill is an authoring and review aid.

It does **not** provide formal ASD certification.

The skill should describe its output as:

* `STE-style`
* `aligned with ASD-STE100 Issue 9`
* `reviewed against ASD-STE100 Issue 9 principles`

The bundled rule references are a working implementation of the standard and are not a reproduction of the complete ASD-STE100 dictionary.

For unusual words where exact dictionary status, approved meaning, or part of speech cannot be established confidently, the skill should identify:

```text
Dictionary verification required.
```

It must not invent dictionary approval.

## Skill structure

```text
ste100/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── core-rules.md
    ├── construction-terminology.md
    └── review-output.md
```

### `SKILL.md`

Defines the trigger conditions, workflow, technical-fidelity requirements, and operating modes.

### `references/core-rules.md`

Contains the working ASD-STE100 Issue 9 rule checklist used for writing and review.

### `references/construction-terminology.md`

Defines how the skill handles construction and electrical technical terminology.

### `references/review-output.md`

Defines the default compliance-review format.

## Standard used

This skill was developed for:

**ASD-STE100 Simplified Technical English**
**Issue 9 — January 2025**
**Standard for technical documentation**

ASD-STE100 Issue 9 is the basis for the writing and review principles implemented by this skill.

## License and ASD-STE100 material

ASD-STE100 is owned by the Aerospace, Security and Defence Industries Association of Europe (ASD).

This skill does not include or reproduce the complete ASD-STE100 standard or controlled dictionary. It contains a practical working summary and instructions derived for use with the skill.

Users who require authoritative interpretation or exact dictionary verification should refer to the official ASD-STE100 Issue 9 publication.

## Purpose

The objective of STE100 is simple:

**Make technical writing easier to read and understand without reducing technical precision or changing project responsibility.**
