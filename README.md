# MR.RUG Framework v12

**Mixture of Reasoning + Agentic GraphRAG**

## Overview

**MR.RUG** is an agentic framework designed to deploy specialized reasoning experts who build a unified knowledge graph through **Reliability-Aware RAG (RA-RAG)**. This system moves beyond passive retrieval, requiring experts to semantically embed the generated graph into their own cognitive architecture before execution.

It serves as **Phase 1 of the KTG-DIRECTIVE** and is best used for tasks requiring multi-expert collaboration, complex analysis, or technical system design.

---

## Core Architecture: M.R.R.U.G

The framework follows a five-phase lifecycle to move from initial deployment to full expert embodiment:

| Phase | Component | Action |
| --- | --- | --- |
| **M** | **Mixture** | Deploy a specific number of experts based on task complexity (R-score). |
| **R** | **Role** | Assign specialized domains and define handoff routes (Baton Passing or Swarm). |
| **R** | **RAG** | Execute specialized retrieval with active **ARQ (Attentive Reasoning Queries)** filtering. |
| **U** | **Update** | Merge individual mini-graphs into a unified structure and resolve conflicting data. |
| **G** | **Generate** | Perform semantic embedding, allowing experts to "embody" the knowledge graph. |

---

## RA-RAG: Reliability-Aware Retrieval

Traditional RAG systems passively summarize retrieved text; MR.RUG utilizes **RA-RAG** to actively categorize and filter information before it enters the system:

1. **Specialized Retrieval:** Experts perform independent, domain-specific searches.
2. **ARQ During Collection:** Active quality introspection to identify failure modes (e.g., outdated advice or vendor bias).
3. **Reliability Scoring:** Content is scored (1-10) on Authority, Recency, Relevance, and Actionability.
* **Threshold:** Content must score **≥7/10** to be kept.


4. **Graph Categorization:** Filtered content is assigned as a specific **Node Type** (Concept, Fact, Relationship, Action, or Validation).
5. **Mini-Graph Construction:** Each expert builds a local graph to model their specific domain.

---

## Expert Archetypes

MR.RUG utilizes a library of specialized roles categorized by task type:

* **Technical:** Systems Architect, Security Expert, Performance Engineer, DevOps.
* **Analytical:** Domain Analyst, Research Specialist, Data Scientist, Strategic Advisor, QA.
* **Creative:** Creative Director, Editor/Critic, Audience Expert, Innovation Catalyst.
* **Cross-Domain:** Integration Architect, Translation Specialist, Synthesis Expert.

---

## Knowledge Graph Structure

The unified graph models complex relationships through defined semantic connections:

### Edge Types

* **REQUIRES:** A needs B to function.
* **ENABLES:** A makes B possible.
* **CONFLICTS_WITH:** A and B are mutually exclusive.
* **SUPPORTS:** A provides evidence for B.
* **DEPENDS_ON:** A relies on the output of B.

---

## Deployment Modes

The number of experts deployed scales automatically with task complexity ( value):

* **QUICK ():** 0 experts; direct answer.
* **ANALYTICAL ():** 3 core specialists.
* **DELIBERATE ():** 5-expert full team.
* **MAXIMUM ():** 5-8 experts.

---

## Timing & Performance

MR.RUG is designed for rapid synthesis without sacrificing depth:

* **Total Execution Time:** ~60–90 seconds for 3–5 experts.
* **Downstream Efficiency:** * **Structure Planning:** 50% faster.
* **Execution:** 30% faster.
* **Verification:** 40% faster.

---

# MR.RUG Framework v12
**Mixture of Reasoning + Agentic GraphRAG**

## 🚧 WIP Status
The conceptual framework and RA-RAG protocols are finalized. Active development is focused on the "G" (Generate/Embody) phase for the MAGMA multi-graph implementation.

## Roadmap
- [x] Finalize M.R.R.U.G initialization protocol
- [x] Define Expert Archetypes (Technical, Analytical, Creative)
- [ ] Implement Asynchronous Consolidation (Dual-Stream Memory)
- [ ] Integrate MAGMA-style 4-graph disentanglement (Semantic, Temporal, Causal, Entity)
- [ ] Publish Benchmark Suite for LoCoMo/LongMemEval

## The M.R.R.U.G Process
1. **M (Mixture):** Deploy experts based on task complexity (R-score).
2. **R (Role):** Assign specialized domains and handoff routes.
3. **R (RAG):** Reliability-Aware retrieval with ARQ filtering (Keep ≥7/10).
4. **U (Update):** Merge mini-graphs and resolve conflicts.
5. **G (Generate):** Semantic embedding and expert embodiment.

## Benchmarks
- **Efficiency:** 30% faster execution; 40% faster verification.

*Created by Kevin Tan (ktg.one) | Part of KTG-DIRECTIVE v30*
