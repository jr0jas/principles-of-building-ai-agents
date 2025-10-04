# Part V – Retrieval and Knowledge Grounding

## Overview
To stay accurate, agents need grounding — connecting to external information sources rather than relying purely on model memory.

## Retrieval-Augmented Generation (RAG)
- Split data into chunks; store embeddings in a vector database.  
- At runtime, retrieve relevant pieces, then generate grounded answers.  
- Manage trade-offs between recall, precision, and context length.

## Agentic RAG
- The agent decides *when* to retrieve, *how much* to retrieve, and *what* to trust.  
- Combines retrieval with reasoning for better judgment.

## Indexing & Embeddings
- Use hybrid search (semantic + keyword).  
- Refresh indexes dynamically when knowledge updates.  
- Store metadata like source, date, confidence.

## Takeaway
Grounding connects reasoning to reality — the agent no longer imagines answers; it *retrieves, verifies, and reasons* over facts.
