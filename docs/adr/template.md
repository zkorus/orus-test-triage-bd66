<!-- orus-version: 0.0.0 -->
# NNNN. <the decision, as one sentence>

<!--
How to use this template:
- Copy this file to docs/adr/NNNN-<short-name>.md, with the next free number, and add a row to the index in README.md.
- List the use cases it serves in the header, and add the ADR's number to those use cases in docs/use-cases.md.
- Remove this comment and every <placeholder>.
- An accepted record is never edited to change its decision; write a new record that supersedes it.
-->

- Status: Proposed | Accepted | Superseded by NNNN
- Implemented: no | partly | yes
- Date: YYYY-MM-DD
- Decided by: <owner>, or "<agent>, delegated by <owner>"
- Use cases: <UC ids this decision serves>
- Supersedes: <NNNN, or remove this line>

## Context

<Where this decision comes from: the use case, the earlier ADR, the review or the problem that raised it, and why it
matters.>

<What is true today, and the constraints any answer must respect. Write it in plain words, for a reader who was not
there and need not know the tools: the problem first, then the facts; explain each technical term the decision turns
on where it first appears. Name only what the repository keeps: no working files, logs or reports kept elsewhere.>

## Question

<The one question this record answers, in a sentence or two.>

## Options

| # | Option | Cost |
|---|---|---|
| 1 | <option> | <what it costs: work, risk, limits, money; measured numbers marked as measured> |
| 2 | <option> | <cost> |

## Decision

**Chosen: option N.** <What happens to each other option: rejected, or deferred to a later record, with a short reason.>

<The decision in words: what is done, and why this option over the others. When it is long, start with a short
"In short" paragraph in plain words, then the details.>

## Consequences

- <What becomes true or required because of this decision.>
- <What later work inherits, and what is still open.>

## Implementation

<Kept up to date by each change that builds part of this decision. "yes" has nothing left, "no" has nothing done,
"partly" has both. A test or source file linked below must name this ADR: a test in its title, "(ADR NNNN)"; a source
file in a comment line, "// Implements: ADR NNNN".>

Done: nothing yet.

Left:

- <What is still to build> (plan step N).
