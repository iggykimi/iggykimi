<p align="center">
  <img src="docs/img/profile-header.svg?v=4" width="100%" alt="Ignacio Montero Gil">
</p>

# Ignacio Montero Gil

Data scientist and AI engineer in Zaragoza, Spain. I build LLM systems, machine learning models and optimisation tools for companies, and I measure how well they work before they ship.

At [Integra Tecnología](https://www.integra3.com) I take client projects from scoping to deployment in banking, industry, healthcare, the public sector and logistics. Before that I automated financial-audit data at KPMG. I studied mathematics at the Universidad de Zaragoza (BSc, and an MSc in Mathematical Modelling, Statistics and Computation).

Client code stays private. What is here are side projects and one benchmark I ran at work and was able to publish, each with its data, tests and limits written down.

## Selected projects

<table>
<tr>
<td width="42%"><a href="https://github.com/iggykimi/iggybench"><img src="docs/img/iggybench.png" alt="Throughput against per-user speed for seven LLMs on one GPU"></a></td>
<td>

**[IggyBench](https://github.com/iggykimi/iggybench)** · Python, vLLM

Seven open-weight LLMs and eleven specialist models on one NVIDIA GB300, over three days. How many chat users one machine serves under a P95 latency target, answer quality per use case with confidence intervals, energy per token and cost per million tokens. Every figure is recomputed from the raw data by scripts in the repo.

</td>
</tr>
<tr>
<td><a href="https://github.com/iggykimi/Arknights-Base"><img src="docs/img/arknights.svg" alt="Daily output of the optimised plan against a greedy assignment"></a></td>
<td>

**[Arknights-Base](https://github.com/iggykimi/Arknights-Base)** · Python, SciPy MILP

A planner for a game's base-building layer. It turns a player's roster into a production model and picks the two-shift staffing with mixed-integer linear programming. Each formula cites the spreadsheet cell it comes from and is tested against the game's own data.

</td>
</tr>
<tr>
<td><a href="https://github.com/iggykimi/catalan-spanish-kindle-dictionary"><img src="docs/img/kindle-coverage.svg" alt="Dictionary coverage measured on real books"></a></td>
<td>

**[Catalan → Spanish Kindle dictionary](https://github.com/iggykimi/catalan-spanish-kindle-dictionary)** · Python

A free dictionary for Kindle e-readers: 54.5k headwords and about 1.1M inflected forms, so conjugated verbs and apostrophe contractions resolve to the right entry. A pipeline merges FreeDict, Softcatalà and Apertium and checks the binary format after every build. Coverage is measured token by token on real books.

</td>
</tr>
<tr>
<td><a href="https://github.com/iggykimi/setrack-web"><img src="docs/img/setrack.jpg" alt="SetRack: logging a set and choosing the next exercise"></a></td>
<td>

**[SetRack](https://github.com/iggykimi/setrack-web)** · TypeScript, React, Capacitor

A gym log for Android, [published on Google Play](https://play.google.com/store/apps/details?id=com.setrack.app). Offline, no account and no internet permission: the data stays on the phone. 11 languages, about 450 automated tests, and layout checks that fail the build when a text overflows in any language. The app code is private; the landing site is public.

</td>
</tr>
<tr>
<td><a href="https://github.com/iggykimi/bidlab"><img src="docs/img/bidlab.jpg" alt="BidLab pricing screen on a real Spanish tender"></a></td>
<td>

**[BidLab](https://github.com/iggykimi/bidlab)** · Python, FastAPI, React

A nine-day hackathon prototype. An LLM reads a Spanish public-tender PDF and proposes requirements with page citations, a person approves them, and a deterministic engine computes price, points and the abnormally-low-offer rule. The model never touches the arithmetic.

</td>
</tr>
</table>

## How I work with coding agents

I write most code with AI agents (Claude Code, OpenCode) and treat them as fast contributors who need a spec and a reviewer. Repos under active work have an `AGENTS.md` with the rules the agent works under: what is generated and must not be edited, which tests gate a change, which numbers come from an external source and must be checked against it. Examples: [Arknights-Base](https://github.com/iggykimi/Arknights-Base/blob/master/AGENTS.md), [BidLab](https://github.com/iggykimi/bidlab/blob/main/AGENTS.md).

The agent writes, and I decide what to build, set the checks and read the results. A change is done when the tests or a reproducible run say so.

## At work

- Multi-agent assistants and conversational systems with LangGraph, running in production for clients
- Document pipelines: OCR plus LLM extraction, integrated with the client's systems
- Natural-language querying over corporate databases
- Predictive models, computer vision and operational optimisation for client problems
- GenAI training for more than 30 companies and public bodies, including LLM agents and Microsoft Copilot adoption

2nd prize at the HACK THE VIBE hackathon, with automatic requirement extraction and eligibility checking over Spanish public tenders. MSc thesis on LLM techniques for predicting the market impact of financial news.

## Open source

Small fixes in the agent tools I use daily, mostly documentation that had drifted from the code: five merged pull requests in [oh-my-pi](https://github.com/can1357/oh-my-pi/pulls?q=is%3Apr+author%3Aiggykimi) (MCP protocol details, Anthropic prompt-caching notes, a Hermes tool-call dialect page).

## Stack

Python · pandas · scikit-learn · PyTorch · SciPy · LangGraph · vLLM · SGLang · FastAPI · Pydantic · PostgreSQL · pgvector · Docker · Azure · TypeScript · React · pytest · Playwright · Ruff

[LinkedIn](https://www.linkedin.com/in/ignacio-montero-gil)
