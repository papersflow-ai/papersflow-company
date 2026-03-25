# Tools

PapersFlow exposes a hosted MCP server at `https://doxa.papersflow.ai/mcp`.

This Agent Company package treats the hosted MCP surface as its shared runtime. Public tools support discovery and verification without premium access. Authenticated tools unlock longer-running research workflows and plotting.

## Public Tools

| Tool | Purpose |
|------|---------|
| search | Generic lookup for papers or identifiers |
| fetch | Return a richer paper record after a search or verification step |
| verify_citation | Verify and normalize a citation string, DOI, URL, PubMed ID, arXiv ID, or title |
| search_literature | Search the literature with a narrower research-oriented interface |
| find_related_papers | Retrieve references, citations, and nearby work for a seed paper |
| get_citation_graph | Build a citation graph around a seed paper |
| get_paper_neighbors | Return grouped one-hop neighbors around a seed paper |
| expand_citation_graph | Expand a previously built graph by one hop |

## Authenticated Tools

| Tool | Purpose |
|------|---------|
| summarize_evidence | Aggregate findings across stored DeepScan history |
| run_deepscan | Start an asynchronous research run |
| get_deepscan_status | Check lightweight run status |
| get_deepscan_live_snapshot | Retrieve richer live progress and partial findings |
| get_deepscan_report | Retrieve the completed DeepScan report |
| run_python_plot | Generate plots from stable report data |

## Source

- Public MCP surface: [papersflow-mcp](https://github.com/papersflow-ai/papersflow-mcp)
- Hosted endpoint: `https://doxa.papersflow.ai/mcp`
