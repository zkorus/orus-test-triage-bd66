<!-- orus-version: 0.0.0 -->
# The development process

This is the development process this repository follows with orus. `orus init` wrote it from orus's process
template; the use cases and the decision records it names are kept in `docs/`.

## The loop

1. **Use case.** The owner writes it and classifies it: must, later or out. Agents may draft, never accept.
2. **ADR.** The question, the numbered options with their costs, the option chosen, and who decided.
3. **Tests.** Written from the use case, failing before the code exists.
4. **Code,** until the tests and the gate pass.
5. **Review,** then small commits, each passing the gate alone.

## Rules

- A change to behaviour, a public interface, a data format or a budget needs a use case, an ADR and a test.
- Every use case traces to at least one ADR and one test.
- A gate is never dropped to make a change pass.
- Evidence (a run, a measurement, a failing case) settles a disagreement, not opinion.
- Agents never merge. Every merge is made by an owner.

## Traceability

Every piece of work can be followed from the need to the release, and back:

| From | To | How |
|---|---|---|
| A use case | its ADRs | the ADRs column of the use-case table, matching each ADR's `Use cases:` line |
| A use case | its tests | the Tests column, listing the test files that name it, such as `(UC-2)` |
| An ADR | its state | `Status` for the decision, `Implemented: no, partly or yes` for the work |
| An ADR | its evidence | the Implementation section: what is done, linking the files and tests, and what is left, with its plan step |
| A test | its ADR | the test names it in its title: `(ADR 0013)` |
| Code | its ADR | a comment line in the file: `// Implements: ADR 0015` |
| A commit | its reason | a last line before the trailers: `Refs: ADR 0019, UC-3, plan step 2` |
| A release | its changes | the changelog entry, naming the issues it fixes |

## Files

| File | Becomes |
|---|---|
| [use-cases.md](../../docs/use-cases.md) | the repository's use cases, with the use-case template at the end |
| [adr/README.md](../../docs/adr/README.md) | the index of the repository's decisions |
| [adr/template.md](../../docs/adr/template.md) | the template for a new decision |
