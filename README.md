# qa-templates

Templates I use for day-to-day QA work. Copy them into a ticket, doc or repo and delete what doesn't apply.

| Template | Use it for |
|---|---|
| [Bug report](templates/bug-report.md) | Filing a defect someone else can reproduce without asking you questions |
| [Test plan](templates/test-plan.md) | Scoping testing for a feature or release |
| [Test cases](templates/test-cases.md) | Writing steps and expected results in a reviewable table |
| [Release checklist](templates/release-checklist.md) | The last pass before shipping to production |
| [Exploratory session](templates/exploratory-session.md) | Time-boxed exploratory testing with notes worth keeping |

The bug report is also set up as a [GitHub issue form](.github/ISSUE_TEMPLATE/bug_report.yml), so it appears when you open a new issue in this repo. Copy the `.github` folder into another repo to get the same form there.

## Principles behind them

- **A bug report is done when a stranger can reproduce it.** Steps, environment, expected vs actual, and evidence.
- **Severity and priority are different questions.** Severity is how bad it is; priority is how soon it gets fixed.
- **Write down what you didn't test.** Out-of-scope lists prevent the "I thought QA covered that" conversation.
- **Evidence beats description.** A screenshot, a HAR file or a status code ends arguments quickly.

MIT licensed. Use them however you like.
