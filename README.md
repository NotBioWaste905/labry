# labry

Local-first research environment for ML. Connect papers, experiments, and writing into one reproducible graph.

## What is labry?

Research is messy. You read papers in Zotero, take notes in Obsidian, run experiments in Jupyter, manage environments with conda, and write in LaTeX — none of which talk to each other. By the time you write the paper, you've forgotten which experiment supported which hypothesis, which citation came from where, and why that one run got better metrics.

labry is a CLI-first tool (and eventually a UI) that treats your research project as a single, structured, git-friendly workspace. Papers, experiments, notes, and manuscripts live in one place, connected by a graph of provenance. Every experiment remembers its code, environment, hardware, and how it relates to your ideas.

Built by an ML researcher, for ML researchers.

## What it does

- Unified workspace — One directory. Papers in `sources/`, experiments in `experiments/`, notes in `notes/`, manuscript in `text/`. All linked.
- Paper management — Add an arXiv URL, get a downloaded PDF, extracted text, auto-fetched BibTeX, and a place for your annotations.
- Reproducible experiments — Every run records the exact code (with git diff), Python version, PyTorch/Transformers versions, GPU, CUDA, and OS. No more "works on my machine".
- Metrics tracking — Experiments write to `metrics.jsonl` with schema validation. Track results across runs without copy-pasting into spreadsheets.
- Graph of knowledge — Link a paper paragraph to a hypothesis, a hypothesis to an experiment, an experiment to a result in your manuscript. Navigate backwards from any figure to its origin.
- Agent-ready — Leave a queue of hypotheses overnight; the agent runs variations, records everything, and reports back.

## Status

**VERY Early development.** The CLI is being built out feature by feature. Core protocol and labry init / source add / experiment run are the current focus. UI, agent, and multi-node SSH workspaces are on the roadmap.
Contributions, issues, and research pain stories are welcome.
