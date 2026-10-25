Trevor Henry

I run Quantum 3 Studio, where I design and ship agentic AI systems for paying clients: LLM orchestration, retrieval, voice agents over live telephony, and encrypted platforms.

Most of that work is under NDA or lives in client accounts, so the repositories here exist to make the claims on my CV checkable. They share a method rather than a subject. Each one measures something rather than demonstrating it, and each publishes the results that went the wrong way.

companies-house-mcp An MCP server over the UK Companies House API, written as an exercise in contract design: tool granularity, response projection, and an error contract a model can branch on.

company-qa-evals Measures whether a model answering from tool results stays grounded in them. The judge has to cite a JSON path that code then resolves, so a fabricated citation downgrades the claim rather than passing.

legislation-rag Retrieval over the Companies Act 2006. Six chunking strategies, hybrid search and reranking measured against a hand-labelled question set. Four of my six predictions were wrong and are published as such.

uk-company-check-skill A Claude skill that answers only from the register and declines to fill the gaps from memory. Built from the failures the eval harness found.

tool-output-injection Whether a model follows instructions hidden in the data its tools return, and which defences actually stop it.

tool results
failure cases
payloads in attacker-chosenfields
companies-house-mcpthe tool surface
company-qa-evalsis the answer grounded
uk-company-check-skillstop the failures found
tool-output-injectionattack the same surface

Four of the five build on each other. The MCP server's output feeds the eval harness, the harness found the failures the skill was written to prevent, and the injection work attacks the same tool surface the server exposes. legislation-rag sits outside that loop: different subject, same insistence on a baseline and a number.

trevor@quantum3.tech
