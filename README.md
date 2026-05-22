# Steve's Prompt Library

Enterprise-grade AI prompts, workflows, and agent instruction sets for Microsoft Copilot, SharePoint Agents, Copilot Studio, and related AI platforms.

---

# Overview

Steve's Prompt Library contains curated and versioned prompts designed for operational, business, and regulated-industry use cases.

This repository focuses on:

* Microsoft 365 Copilot
* SharePoint Agents
* Copilot Studio
* GPT-4o
* Claude Opus
* Enterprise AI workflows
* RFP analysis
* Risk extraction
* Executive productivity
* Security and compliance review
* Justice and corrections workflows

These prompts are treated as managed operational assets rather than disposable text snippets.

---

# Repository Structure

```text
/copilot-prompts
    /executive
    /sales
    /security
    /rfp
    /justice

/sharepoint-agents
    /risk-extraction
    /compliance-review
    /document-analysis

/copilot-studio
    /agents
    /topics
    /actions

/templates
    /metadata
    /yaml
    /json
```

---

# Prompt Package Structure

Each prompt package typically contains:

```text
README.md
prompt.md
metadata.json
examples.md
CHANGELOG.md
```

Example:

```text
/copilot-prompts/rfp-risk-analysis/
```

---

# Design Philosophy

This repository follows several core principles:

## 1. Prompts Are Software Assets

Prompts should be:

* versioned
* documented
* tested
* repeatable
* maintainable

## 2. Platform-Specific Optimization Matters

Prompts behave differently across:

* Microsoft 365 Copilot
* SharePoint Agents
* GPT-4o
* Claude Opus
* Copilot Studio

Each platform may require:

* different instruction structures
* different context management
* different output formatting
* different token optimization strategies

## 3. Enterprise Reliability Over Creativity

These prompts prioritize:

* consistency
* explainability
* operational accuracy
* reduced hallucinations
* governance
* auditability

---

# Versioning

This repository uses Semantic Versioning.

Format:

```text
MAJOR.MINOR.PATCH
```

Examples:

| Version | Meaning                         |
| ------- | ------------------------------- |
| 1.0.0   | Initial production release      |
| 1.1.0   | New capability added            |
| 1.1.1   | Minor fix or wording refinement |

---

# Releases

Prompt updates are distributed through GitHub Releases.

Each release includes:

* updated prompts
* release notes
* compatibility updates
* known limitations
* breaking changes (if applicable)

Users are encouraged to:

* Watch the repository
* Subscribe to releases
* Review changelogs before deployment

---

# Supported Platforms

Current prompt packs may support one or more of:

* Microsoft 365 Copilot
* SharePoint Agents
* Copilot Studio
* ChatGPT
* Claude Opus
* Azure OpenAI
* Azure AI Foundry

Compatibility is documented within each prompt package.

---

# Example Metadata

Example `metadata.json`:

```json
{
  "promptId": "rfp-risk-analyzer",
  "version": "1.4.0",
  "author": "Steve McPherson",
  "compatibleModels": [
    "gpt-4o",
    "claude-opus"
  ],
  "platforms": [
    "Microsoft 365 Copilot",
    "SharePoint Agents"
  ],
  "lastUpdated": "2026-05-22"
}
```

---

# Testing Philosophy

Prompts should be validated against:

* multiple document sizes
* varying context windows
* hallucination scenarios
* edge-case inputs
* platform truncation limits

Where applicable, prompts may include:

* expected outputs
* evaluation examples
* known failure modes

---

# Known Considerations

## SharePoint Agent Limitations

SharePoint Agents may:

* truncate large documents
* limit contextual reasoning depth
* reduce extraction accuracy on long RFPs

For large document analysis:

* staged prompt chains are recommended
* chunking strategies may be required

## Model Variance

Claude Opus and GPT-4o may produce materially different results using the same instructions.

Prompts may include:

* model-specific variants
* model tuning notes
* platform recommendations

---

# Licensing

Unless otherwise stated:

* Public prompts are provided for educational and operational use.
* Enterprise implementations may require separate licensing.
* Redistribution of modified commercial prompt packs may be restricted.

See individual folders for licensing details.

---

# Contributions

Contributions, issues, refinements, and testing feedback are welcome.

Areas of interest:

* enterprise AI governance
* RFP automation
* compliance review
* security analysis
* workflow orchestration
* regulated-industry AI systems

---

# About This Repository

This repository is focused on practical AI workflow systems and enterprise prompt engineering for real-world operational environments.

Primary focus areas include:

* Microsoft Copilot integrations
* SharePoint Agent optimization
* document intelligence
* AI workflow orchestration
* executive productivity
* regulated-industry AI solutions
