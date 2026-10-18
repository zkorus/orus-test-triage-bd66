<!-- orus-version: 0.0.0 -->
# Decision records

Each record answers one question: the options with their costs, the decision, and who made it. A record is
**Proposed** until the owner accepts it. An accepted record is never edited to change its decision; a new record
supersedes it.

**Status** tracks the decision; **Implemented** tracks the work: `no`, `partly` or `yes`, with what is done and what
is left in each record's Implementation section.

| ADR | Decision | Status | Implemented |
|---|---|---|---|

## Template

New records start from [template.md](template.md). A Context section tells where the decision comes from and why it
was needed, for a reader who was not there. Every option is numbered, and the decision opens with the number
of the option chosen ("option N", "options N and M", or "option N now, option M later"), so the choice is clear
without reading the prose. The Implementation section says what is done, with its evidence, and what is left.
