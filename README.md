# Reports to axKit

Bugs, feature requests and feedback about [axKit](https://github.com/KyleKeane/AxKit), a set of accessible Windows apps
for a blind developer who uses the NVDA screen reader, shared in case they help others.

## How a report gets here

Most issues here are sent from inside axKit: F4 in any of its windows (or axKit menu, Send a report) opens a report,
the user types a few words and presses Enter. The report is saved on the user's computer first and then posted here
as an issue by axKit's own account, `axkit-reporter`, so that nobody has to sign in. It ends with one line,
`Sent from axKit <version> with F4; reporter <id>`, where the id is a random id of that install of axKit, not of a
person. What else a report carries, and what never does, is said in axKit's
[PRIVACY.md](https://github.com/KyleKeane/AxKit/blob/main/PRIVACY.md) and in the design,
[docs/axkit/reports.md](https://github.com/KyleKeane/AxKit/blob/main/docs/axkit/reports.md).

Anyone with a GitHub account can also file an issue here directly, with the Bug report or Idea form.

## Labels

`bug`, `feature` and `feedback` are the three kinds a report is sent as; the maintainer changes them as needed. Work
that is taken up moves to the code repository, [KyleKeane/AxKit](https://github.com/KyleKeane/AxKit/issues).

## blocklist.json

Reports from an install or an axKit version that sends nonsense can be stopped: `blocklist.json` at the root of this
repository lists reporter ids and versions. axKit reads it before sending and sends nothing for a listed one; the
workflow in `.github/workflows/close-blocked.yml` closes and locks a listed report that arrives anyway. The maintainer
edits the file from axTask (Block this reporter, Block this version) or by hand.

## Maintenance

How this repository, the reporter account and its token are set up and renewed is
[docs/axkit/reports-setup.md](https://github.com/KyleKeane/AxKit/blob/main/docs/axkit/reports-setup.md) in the code
repository. axKit is made by Dr. Kyle Keane, www.kylekeane.com.
