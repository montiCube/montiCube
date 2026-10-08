# Jake Raum

I build software by directing AI coding agents. I write the task specs, set the gates a change has to pass, and decide what merges. Based in Portsmouth, NH.

## antsPholio (private repository)

An automated trading engine that runs against a **paper account**. No real money is deployed. The code is private, so this page describes how it is built and run.

**Stack:** Python, FastAPI, SQLite, Alpaca API, GitHub Actions, nginx. The trader runs on a DigitalOcean server, and research and backtesting run on a separate Ubuntu machine.

### How the work gets done

- About 200 pull requests, written by AI coding agents (mostly Claude Code) from briefs I write.
- Each agent session works in its own git worktree. Agents can push branches and open pull requests. Only I merge to main.
- Every change has to pass a CI gate of more than 3,000 tests. Branch protection has no admin bypass.
- Behavioral changes land together with an entry in a decision log, which now has more than 200 entries.
- A seven-role adversarial review audits the system and my own write-ups: independent agent reviewers, blind verification of every finding, then a red-team pass. It has caught documents of mine claiming things the code did not do, and I corrected them.

### What I'm improving

Most of my verification so far has been ruling on evidence that agents gather for me. I now read diffs by hand every day, starting with past bug fixes, so that I can check a finding myself.

**Workflow sample:** [gist title](GIST_URL)

## Also

Early Three.js and WebGL prototypes aimed at Rokid AR glasses.

## Contact

- Email: jakeraum@gmail.com
- LinkedIn: [ian-jacob-raum](https://linkedin.com/in/ian-jacob-raum-934164246)
