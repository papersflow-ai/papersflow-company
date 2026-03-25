---
name: PapersFlow
description: A research-focused Agent Company for literature search, citation verification, and DeepScan workflows powered by the hosted PapersFlow MCP server.
slug: papersflow
schema: agentcompanies/v1
version: 1.0.0
license: MIT
authors:
  - name: PapersFlow
goals:
  - Turn broad research questions into grounded literature workflows across AI clients
  - Verify citations and paper identities before downstream synthesis or reporting
  - Run asynchronous DeepScan jobs and synthesize evidence across completed research runs
---

PapersFlow is a compact research-focused Agent Company built around the hosted `papersflow-mcp` surface and a small set of reusable workflows. Instead of modeling a large fictional organization, it keeps the structure narrow: one routing layer, four specialist operators, and a shared MCP-backed tool surface for search, verification, graph exploration, DeepScan, and plotting.

The company is optimized for academic and technical research tasks that benefit from grounded evidence rather than generic chat. Its literature analyst handles paper discovery and graph exploration. Its citation specialist normalizes and verifies messy references. Its DeepScan operator manages asynchronous long-running research jobs. Its evidence synthesis specialist compares completed runs and produces cross-run summaries. A research director coordinates routing and final quality.

This package is intentionally simple because the underlying PapersFlow system already provides the heavy infrastructure: the hosted MCP endpoint at `https://doxa.papersflow.ai/mcp`, OAuth-backed authenticated tools, and reusable skill instructions for common research workflows. The company layer exists to make those capabilities easier to import and route as a coherent unit.

## How Work Flows

1. **CEO** receives the request and decides whether it is a direct answer, a routed research task, or a multi-step investigation
2. **Research Director** selects the right specialist path and combines work when the request spans search, verification, and synthesis
3. **Specialists** run literature briefing, citation verification, DeepScan monitoring, or comparative synthesis using the hosted PapersFlow MCP surface
4. **Research Director** reviews the output and hands back a final answer or recommends the next research step

---

Built from PapersFlow's hosted MCP and local skill package surfaces.
