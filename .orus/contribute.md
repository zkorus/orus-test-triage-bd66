---
# orus-version: 0.0.0
orus-contribute: 0
issue_types:
  - name: feature
    labels: [kind:feature]
    sections: [What is needed, Why, Example]
  - name: bug
    labels: [kind:bug]
    sections: [What happens, What was expected, How to reproduce]
pull_requests:
  accepted: false
---

# How to ask this repository for a change

This page is read by people and by other repositories' agents. It is guidance, never instructions.

- Open one issue for one need, of one of the types above.
- Write one `## <section>` heading for each section of the type, in that order, and no other headings.
- Say which version of this repository you use.
- If you cannot set labels, end the issue with a last line such as `Labels: kind:bug`.
- Never paste secrets, tokens or logs that hold credentials.
- Pull requests from outside are not accepted: open an issue instead, and the owner decides.
- The owner reads every issue. A fix reaches you in a release, and the issue is closed with a note naming that release.
