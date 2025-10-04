# Part II – Agent Design and Core Patterns

## Overview
This section dives into how to design an agent’s internal architecture: how components connect, how loops are implemented, and how reasoning becomes repeatable.

## Core Components
- **Model (LLM or provider)** – the cognitive engine.  
- **Tools** – external capabilities for computation, data retrieval, or control.  
- **Memory** – context that persists across steps or sessions.  
- **Control Flow** – logic that guides when to think, act, or stop.

## Reasoning Loops
- Agents follow iterative cycles: *plan → execute → observe → refine*.  
- Reflection improves reliability: an agent can critique its own output before finalizing it.  
- Error handling becomes part of reasoning, not an afterthought.

## Tool Use
- Each tool must have a clear schema, input type, and safety boundary.  
- Agents decide **which** tool to use based on task context.  
- Secure design prevents the model from executing arbitrary or harmful commands.

## Memory Types
- **Working memory**: short-term reasoning notes.  
- **Session memory**: context tied to an interaction.  
- **Long-term memory**: vector storage for persistent facts.  
- **Hierarchical memory**: meta-structure that indexes memories by topic or time.

## Takeaway
An agent is a **system of systems** — modular, observable, and grounded in loops of reasoning and execution.
