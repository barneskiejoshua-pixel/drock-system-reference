# DRock system reference

A ground-up reference for DRock, a computer-use agent built around a small local model (0.6B to 4B
parameters in Ollama) and a deterministic executor. The model proposes one action at a time; the
executor runs it and checks the result against the machine; a completion gate decides from the
request's own text when the task is actually done.

- `DRock-System-Reference.pdf`: the document (20 pages)
- `DRock-System-Reference.html`: its source

It covers the agent loop, the 114-action protocol, the executor, the completion gate, policy and
safety layers, the no-model fast paths, the chat layer, models and GPU serving, memory and
knowledge, measurement, the development tooling, the design rules, the bugs that shaped it, a
command reference, open work, and an index of all 102 modules.

Numbers were read from the source tree and its logs on 2026-11-20. The source itself is not in
this repository.
