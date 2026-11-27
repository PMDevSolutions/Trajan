# Trajan

One desktop app, with one installer per operating system, for the PMDS Claude Code toolkits:

- [Flavian](https://github.com/PMDevSolutions/Flavian), WordPress development
- [Aurelius](https://github.com/PMDevSolutions/Aurelius), React apps
- [Vespasian](https://github.com/PMDevSolutions/Vespasian), Wix Studio sites
- [Nerva](https://github.com/PMDevSolutions/Nerva), APIs and backends
- [Claudius](https://github.com/PMDevSolutions/Claudius), a chat widget that answers with Claude

Named after Emperor Trajan, like its siblings are named after theirs.

## Status

**Not released, and there is no code in this repository yet** (2026-11-25).

Trajan will be built from the Electron and React desktop app that lives in Flavian's
[`packages/gui`](https://github.com/PMDevSolutions/Flavian/tree/main/packages/gui). Flavian, Aurelius
and Vespasian each carry a copy of that engine today. The copies are being folded back into one, and
the engine moves here once they are.

| Step | State |
| --- | --- |
| One manifest contract for Flavian, Aurelius and Vespasian | Done ([Flavian #196](https://github.com/PMDevSolutions/Flavian/pull/196)) |
| Vespasian's Wix-site screen in the shared engine | To do ([#2](https://github.com/PMDevSolutions/Trajan/issues/2)) |
| Aurelius's additions and a generic step runner | To do ([#2](https://github.com/PMDevSolutions/Trajan/issues/2)) |
| Product-neutral transport and build identity | To do ([#2](https://github.com/PMDevSolutions/Trajan/issues/2)) |
| The engine moves to this repository; Aurelius and Vespasian adopt it | To do ([#2](https://github.com/PMDevSolutions/Trajan/issues/2), [#4](https://github.com/PMDevSolutions/Trajan/issues/4)) |
| Choosing a product at run time, and starting a new project from a template | To do ([#3](https://github.com/PMDevSolutions/Trajan/issues/3)) |
| Nerva and Claudius manifests | To do ([#5](https://github.com/PMDevSolutions/Trajan/issues/5), [#6](https://github.com/PMDevSolutions/Trajan/issues/6)) |

## Where the work happens until then

The issues are tracked here. The code stays in Flavian until the engine moves, so pull requests for the
engine are opened in Flavian and say "Part of PMDevSolutions/Trajan#2".

- The epic: [#1](https://github.com/PMDevSolutions/Trajan/issues/1)
- The engine work: [#2](https://github.com/PMDevSolutions/Trajan/issues/2), with its
  [design](https://github.com/PMDevSolutions/Flavian/blob/main/docs/plans/2026-11-08-trajan-engine-reconciliation-design.md)
  and [plan](https://github.com/PMDevSolutions/Flavian/blob/main/docs/plans/2026-11-08-trajan-engine-reconciliation-plan.md)
  in Flavian
- How the engine, the manifests and the panels fit together:
  [`GUI-PLATFORM.md`](https://github.com/PMDevSolutions/Flavian/blob/main/packages/gui/docs/GUI-PLATFORM.md)
- [Every open issue](https://github.com/PMDevSolutions/Trajan/issues)

## If you want the desktop app today

Flavian and Aurelius attach installers of their own builds to their releases (an AppImage, two DMGs and
a Windows installer each):

- [Flavian releases](https://github.com/PMDevSolutions/Flavian/releases)
- [Aurelius releases](https://github.com/PMDevSolutions/Aurelius/releases)

The builds are unsigned, so Windows and macOS warn on first launch.

## License

[MIT](LICENSE)
