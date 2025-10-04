# Part III – Tool Ecosystem and Protocols

## Overview
Agents gain power through tools — external APIs, databases, browsers, or functions. This part establishes conventions for connecting them safely and efficiently.

## Tool Interfaces
- Define tool purpose, parameters, and expected outputs.  
- Keep inputs minimal and explicit.  
- Add metadata (auth, rate limits, error types).

## Patterns
- **Reason + Act**: the model explains reasoning before choosing a tool.  
- **Tool feedback loop**: results from the tool are re-fed into the next reasoning step.  
- **Composable tools**: each tool performs one atomic action.

## Model-Context Protocol (MCP)
- Standard for communication between agents and tools.  
- Unifies schema definitions, execution, and context sharing.  
- Supports interoperability across languages and frameworks.

## Safety and Governance
- Restrict access by capability (principle of least privilege).  
- Log every tool call for observability.  
- Validate tool responses before using them downstream.

## Takeaway
Tool use transforms language models into **actors** — systems that can interact with the world through well-defined, auditable interfaces.
