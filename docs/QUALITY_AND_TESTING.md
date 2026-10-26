# Soc Ops Python Agent Lab: Development and QA Guide

This repository contains a social-bingo activity and guided materials for learning agent-oriented development workflows. The README points learners to a step-by-step workshop guide; use the checked-in Python source and guide as the authority for the current features.

## Setup

```bash
git clone https://github.com/kandisaikishore/agent-lab-python.git
cd agent-lab-python
```

Inspect the Python project files to identify the supported Python version, dependency manager, entry point, and test commands. Create an isolated virtual environment and install only the declared dependencies. Keep API keys and local environment files out of commits.

## Social-bingo QA

For implemented game flows, test:
- Creating or loading a participant card
- Matching prompts to participants
- Duplicate matches and invalid/empty participant data
- Completion of five-in-a-row logic
- Empty participant lists and malformed inputs
- Reset/restart behavior and clear feedback

Use deterministic fixture participants rather than real attendee data.

## Agent-lab exercises

For each workshop step, document prerequisites, expected input/output, and a way to verify completion. Mark any provider-dependent exercise that requires credentials or external access. Do not claim a model call or external tool succeeded unless it was actually executed.

## Safety and privacy

Use synthetic prompts and data in tests. Do not commit secrets, private workshop attendee information, or logs containing credentials. Where agent tools can modify files or external resources, document permissions and expected side effects.

## Pull-request checklist

- [ ] Run the available Python tests/lint/type checks from project configuration.
- [ ] Add regression tests for changed behavior.
- [ ] Verify workshop instructions from a clean environment where possible.
- [ ] State which external provider steps were mocked or skipped.
- [ ] Keep examples and outputs reproducible.
