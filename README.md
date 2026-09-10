<<<<<<< HEAD
# System Design for AI/ML

A personal study and portfolio repo for System Design applied to ML, GenAI, and Agentic systems — built to prepare for ML Engineer / AI Engineer / GenAI Engineer interviews.

**Author:** Gilson Vieira de Souza — Machine Learning Engineer (GenAI & AI Engineering)
**Companion repo:** [`language-ai-engineering-lab`](#) — conceptual/learning notebooks live there; this repo is applied design + interview prep.

---

## Why this structure

Most "system design" prep treats every topic as equally weighted. This roadmap instead follows a deliberate progression:

```
Software System Design → ML System Design → GenAI System Design → Agentic System Design
```

Each phase builds on the last, and maps directly onto real experience (Spring Boot/Kafka/Terraform → SageMaker/MLflow → LangChain/RAG → LangGraph/MCP), so studying doubles as articulating what I already do in production.

Every completed case follows the same 15-point structure (see [`_templates/design-doc-template.md`](_templates/design-doc-template.md)), so depth is comparable across topics and the format becomes second nature under interview pressure.

---

## Progress tracker

### Phase 0/1 — Fundamentals (refresher, not deep study)
- [ ] Scalability, availability, reliability, CAP theorem
- [ ] Load balancing, caching, queues, API design
- [ ] Architecture patterns: CQRS, Saga, circuit breaker, rate limiting

### Phase 2 — ML System Design
- [ ] ML lifecycle: ingestion → feature store → training → serving → monitoring
- [ ] Batch vs. online inference
- [ ] Data/concept drift, retraining, A/B & canary/shadow deployment
- **Cases:**
  - [ ] `fraud-detection.md`
  - [ ] `recommendation-system.md`
  - [ ] `ml-inference-platform.md`

### Phase 3 — GenAI System Design
- [ ] LLM serving, routing, prompt & context management, token budgeting
- [ ] RAG: embeddings, chunking, retrieval, reranking, hybrid search
- [ ] Evaluation, hallucination mitigation, guardrails, cost/latency optimization
- **Cases:**
  - [ ] `rag-for-millions-users.md`
  - [ ] `enterprise-ai-assistant.md`
  - [ ] `llm-evaluation-platform.md`

### Phase 4 — Agentic System Design
- [ ] Agent architecture, tool calling, ReAct, memory (short/long-term)
- [ ] Multi-agent orchestration, human-in-the-loop, MCP, tool registry
- [ ] Agent evaluation, tracing, failure recovery, cost/latency control
- **Cases:**
  - [ ] `multi-agent-customer-support.md`
  - [ ] `mcp-enterprise-agent-platform.md`

---

## Repo structure

```
system-design-ai/
│
├── README.md
├── 00-fundamentals/
│   └── notes.md
├── 01-ml-system-design/
│   ├── notes.md
│   └── cases/
├── 02-genai-system-design/
│   ├── notes.md
│   └── cases/
├── 03-agentic-system-design/
│   ├── notes.md
│   └── cases/
├── _templates/
│   └── design-doc-template.md
└── diagrams/
```

- **`notes.md`** per phase — condensed reference notes, not a folder-per-concept. Searchable, not sprawling.
- **`cases/`** — completed design docs. This is the portfolio: what a recruiter or interviewer would actually open.
- **`_templates/`** — one reusable design doc template, applied consistently to every case.
- **`diagrams/`** — architecture diagrams referenced by relative path from cases, centralized so formats stay consistent.

## How to use this repo

1. Pick a case from an unstarted phase.
2. Copy `_templates/design-doc-template.md` into the phase's `cases/` folder, rename it.
3. Fill it out end-to-end — no skipping sections, even weak ones. Weak sections reveal what to study next.
4. Check it off above.
=======
# System Design Ai



## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Add your files

* [Create](https://docs.gitlab.com/user/project/repository/web_editor/#create-a-file) or [upload](https://docs.gitlab.com/user/project/repository/web_editor/#upload-a-file) files
* [Add files using the command line](https://docs.gitlab.com/topics/git/add_files/#add-files-to-a-git-repository) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.com/gil-son/system-design-ai.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

* [Set up project integrations](https://gitlab.com/gil-son/system-design-ai/-/settings/integrations)

## Collaborate with your team

* [Invite team members and collaborators](https://docs.gitlab.com/user/project/members/)
* [Create a new merge request](https://docs.gitlab.com/user/project/merge_requests/creating_merge_requests/)
* [Automatically close issues from merge requests](https://docs.gitlab.com/user/project/issues/managing_issues/#closing-issues-automatically)
* [Enable merge request approvals](https://docs.gitlab.com/user/project/merge_requests/approvals/)
* [Set auto-merge](https://docs.gitlab.com/user/project/merge_requests/auto_merge/)

## Test and Deploy

Use the built-in continuous integration in GitLab.

* [Get started with GitLab CI/CD](https://docs.gitlab.com/ci/quick_start/)
* [Analyze your code for known vulnerabilities with Static Application Security Testing (SAST)](https://docs.gitlab.com/user/application_security/sast/)
* [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/topics/autodevops/requirements/)
* [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/user/clusters/agent/)
* [Set up protected environments](https://docs.gitlab.com/ci/environments/protected_environments/)

***

# Editing this README

When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thanks to [makeareadme.com](https://www.makeareadme.com/) for this template.

## Suggestions for a good README

Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.

## Name
Choose a self-explaining name for your project.

## Description
Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.

## Badges
On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.

## Visuals
Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.

## Installation
Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.

## Usage
Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.

## Support
Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.

## Roadmap
If you have ideas for releases in the future, it is a good idea to list them in the README.

## Contributing
State if you are open to contributions and what your requirements are for accepting them.

For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.

You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.

## Authors and acknowledgment
Show your appreciation to those who have contributed to the project.

## License
For open source projects, say how it is licensed.

## Project status
If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
>>>>>>> dd8f20f5a12c569569752f427c9dafa93b847d4a
