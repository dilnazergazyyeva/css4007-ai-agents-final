## Week 10 Progress Report

## Completed Work

- Forked the instructor repository and cloned it.
- Read the A-level requirements and the guardrail rules.
- Chose the project: a deadline planner agent for students.
- Wrote the proposal (`reports/proposal.md`): problem, tools, architecture, 12 planned tests and a plan for each week.

## Important Commits

- Commit hash: 0d0110f
- Description: Add project proposal for the deadline planner agent
- Link: https://github.com/dilnazergazyyeva/css4007-ai-agents-final/commit/0d0110fcc0cd7df0da4ea368a03cf868c691df62

## Current Functionality

There is no working application yet. This week was planning only. The repository has the proposal and this report.

## Problems Encountered

I did not have a topic at first. It was hard to see what makes an A-level agent different from a simple chatbot with tools.

## Solutions

I compared a few topic ideas and picked the one where all guardrails fit naturally: read-only tools, one tool that writes a file and needs approval, and mock data where I can add a malicious note for the injection test. To understand A level, I turned the requirements into a short list: tools, state, limits, validation, approval, trace, tests.

## What I Learned

An agent is not just a model with tools. The program around the model decides what is allowed. If a rule only exists in the prompt, the model can break it. If it is checked in code, it cannot. I also learned that text from documents has to be treated as data and not as instructions, because a document can try to give commands to the agent.

## Next Week

- Create `.env` from `_env.example` and make sure it is not committed.
- Make the mock data file with students, courses and deadlines (one course with no deadlines).
- Connect the LLM API and get the first working request.
- Start the project README.
