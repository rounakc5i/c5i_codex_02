---
name: checkout-tests
description: Use when changing, adding, or removing application code or functions in the Tiny Shop Checkout starter; run its unittest suite after the code change.
---

# Verify Tiny Shop code changes

When a task changes application code or a function in this starter, run the complete documented test suite after the edits, including when tests were also changed. From `learner/starter/`, use:

```sh
python3 -m unittest discover -s tests -v
```

Report whether the command passed, failed, or could not run. If it fails, include the relevant failure output and do not describe the change as verified. Documentation-only changes do not trigger this skill. Do not modify application code solely to make the test command available; report the blocker instead.
