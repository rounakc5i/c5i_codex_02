# Repository guidance

## Purpose and public contract

- This repository is a self-contained training lab about project guidance, Skills, MCP grounding, and review (`README.md`).
- The learner starter is a small Python checkout example (`learner/starter/README.md`).
- Its public function is `calculate_total(items)`: it sums `float(item["price"]) * int(item["quantity"])` for each item and returns a float (`learner/starter/src/checkout.py`).
- Keep existing calls and the documented item inputs in mind when changing checkout behavior. The visible tests cover a single item, multiple items, an empty cart, and the float return type (`learner/starter/tests/test_checkout.py`).

## Working rules

- Keep checkout implementation in `learner/starter/src/` and its tests in `learner/starter/tests/`, consistent with the starter project map (`learner/starter/README.md`).
- Do not add dependencies for starter exercises; the starter README says no package installation is required (`learner/starter/README.md`).
- The checkout exercise uses floats. Its source docstring notes that production money code would normally use `Decimal` or integer minor units; do not treat that note as a request to change this exercise's contract (`learner/starter/src/checkout.py`).
- Make only changes requested by the current task. Task cards describe exercise requirements, not changes already made to the starter (`learner/starter/task_card.md`).

## Verification

From `learner/starter/`, run:

```sh
python3 -m unittest discover -s tests -v
```

This is the verification command documented by the starter README (`learner/starter/README.md`).

## Scope and ambiguity

- The learner starter intentionally has no `AGENTS.md`; this repository-root file provides repository-level guidance (`learner/starter/README.md`).
- The repository README mentions instructor materials, but those paths are not present in this checkout's file listing (`README.md`). Do not assume their contents or use them as an implementation requirement.
- If a task conflicts with the observed checkout contract or its tests, identify the conflict and ask for clarification before changing that contract. For other ambiguities, state the assumption and use the existing source, tests, and documented command as evidence.
