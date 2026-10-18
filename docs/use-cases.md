<!-- orus-version: 0.0.0 -->
# Use cases

Only the owner accepts a use case, classifies it (must, later, out) or changes an accepted one.

Each use case traces to at least one ADR and, once code exists, to at least one test. New use cases follow the
[template](#template) at the end of this file.

| Id | Use case | Class | ADRs | Tests | Status |
|---|---|---|---|---|---|
| UC-1 | Divide one number by another | must | | | accepted |

## UC-1. Divide one number by another

**Actor:** calculator user. **Goal:** divide one number by another.

1. The user enters a dividend and a divisor.
2. orus returns the quotient of the dividend divided by the divisor.
3. When the divisor is zero, orus reports an error and returns no quotient.

**Done when:** for a dividend and a non-zero divisor, the returned quotient equals the dividend divided by the divisor, and for a zero divisor an error is reported and no quotient is returned.

For #2.

## Template

To add a use case:

1. Take the next free id and add a row to the table above: the class empty (or proposed, when an agent drafts it),
   the ADRs and tests empty until they exist, the status `draft`.
2. Copy the block below to the end of the list of use cases, before this section, and replace every `<placeholder>`.

```markdown
## UC-N. <what the actor can do, as a short sentence>

**Actor:** <who acts: a person's role or an agent>. **Goal:** <what they want, in their terms>.

1. <a step: who does what, as seen from outside>
2. <a step>

**Done when:** <a condition that can be checked, so a test can trace to it>.

For #<issue>.
```

Rules:

- **One goal per use case.** If the steps serve two goals, write two use cases.
- **What, not how.** Steps say what the actor and orus do, as seen from outside; formats and designs belong in ADRs.
- **Checkable.** "Done when" must be something a test or a run can show, never "works well".
- **The link to an issue.** The last line, `For #<issue>.`, names the issue the use case answers, by its number;
  for another issue, add its number to that line (`For #7, #9.`), never a second line. Leave it out when there is none.
  Once the use case is `accepted`, this line is what lets orus mark the issue ready for Dev; no other mention of the
  issue links it.
- **The owner decides.** An agent may write a use case only as `draft` and may only propose its class. Only the owner
  sets the class (must, later, out) and the status `accepted`, and an accepted use case changes only by the owner.
