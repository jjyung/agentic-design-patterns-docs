# Agentic Design Patterns - Complete Reference

This directory contains 21 integrated agentic design patterns, each combining detailed discussion with visual flow diagrams.

## What's Inside Each Pattern

Every pattern file includes:

- **When to Use**: Specific scenarios and use cases
- **Visual Flow**: Interactive Mermaid diagram showing the process
- **Where It Fits**: Application domains and contexts
- **Pros**: Advantages and benefits
- **Cons**: Limitations and challenges
- **Real-World Examples**: Practical implementation scenarios
- **Original Files**: References to source documentation

## Quick Navigation

### Core Patterns (01-05)

Essential foundational patterns for building agentic systems.

| #   | Pattern                                      | Description                                  |
| --- | -------------------------------------------- | -------------------------------------------- |
| 01  | [**Prompt Chaining**](01-prompt-chaining.md) | Breaking complex tasks into sequential steps |
| 02  | [**Routing**](02-routing.md)                 | Directing requests to the right handler      |
| 03  | [**Parallelization**](03-parallelization.md) | Running multiple tasks simultaneously        |
| 04  | [**Reflection**](04-reflection.md)           | Self-evaluation and improvement              |
| 05  | [**Tool Use**](05-tool-use.md)               | Integrating external capabilities            |

### Advanced Patterns (06-10)

Sophisticated patterns for complex workflows and coordination.

| #   | Pattern                                                          | Description                      |
| --- | ---------------------------------------------------------------- | -------------------------------- |
| 06  | [**Planning**](06-planning.md)                                   | Strategic task decomposition     |
| 07  | [**Multi-Agent Collaboration**](07-multi-agent-collaboration.md) | Coordinating multiple agents     |
| 08  | [**Memory Management**](08-memory-management.md)                 | Storing and retrieving context   |
| 09  | [**Learning and Adaptation**](09-learning-and-adaptation.md)     | Improving over time              |
| 10  | [**Model Context Protocol**](10-model-context-protocol.md)       | Standardized agent communication |

### System Patterns (11-15)

Infrastructure patterns for production-ready systems.

| #   | Pattern                                                                      | Description                  |
| --- | ---------------------------------------------------------------------------- | ---------------------------- |
| 11  | [**Goal Setting and Monitoring**](11-goal-setting-and-monitoring.md)         | Tracking objectives          |
| 12  | [**Exception Handling and Recovery**](12-exception-handling-and-recovery.md) | Graceful error management    |
| 13  | [**Human-in-the-Loop**](13-human-in-the-loop.md)                             | Incorporating human feedback |
| 14  | [**Knowledge Retrieval (RAG)**](14-knowledge-retrieval-rag.md)               | Accessing external knowledge |
| 15  | [**Inter-Agent Communication (A2A)**](15-inter-agent-communication-a2a.md)   | Agent-to-agent messaging     |

### Optimization Patterns (16-19)

Performance and safety-focused patterns.

| #   | Pattern                                                              | Description                    |
| --- | -------------------------------------------------------------------- | ------------------------------ |
| 16  | [**Resource-Aware Optimization**](16-resource-aware-optimization.md) | Efficient resource usage       |
| 17  | [**Reasoning Techniques**](17-reasoning-techniques.md)               | Structured thinking approaches |
| 18  | [**Guardrails/Safety Patterns**](18-guardrails-safety-patterns.md)   | Ensuring safe operations       |
| 19  | [**Evaluation and Monitoring**](19-evaluation-and-monitoring.md)     | Performance tracking           |

### Strategic Patterns (20-21)

High-level patterns for decision-making and exploration.

| #   | Pattern                                                          | Description              |
| --- | ---------------------------------------------------------------- | ------------------------ |
| 20  | [**Prioritization**](20-prioritization.md)                       | Managing task importance |
| 21  | [**Exploration and Discovery**](21-exploration-and-discovery.md) | Finding new solutions    |

## How to Use This Reference

1. **Browse by Category**: Start with the category that matches your needs
2. **View Visual Flows**: Each pattern includes an embedded Mermaid diagram
3. **Check Examples**: Real-world scenarios help understand practical applications
4. **Review Trade-offs**: Pros and cons help you make informed decisions
5. **Access Sources**: Original files available for detailed study

## Additional Resources

- **ASCII Art Diagrams**: See [../ascii-art](../ascii-art) for text-based versions
- **Standalone Mermaid**: See [../mermaid-diagrams](../mermaid-diagrams) for diagram source files
- **Detailed Discussions**: See [../pattern-discussion](../pattern-discussion) for original markdown files

## Pattern Selection Guide

**Starting a new project?** Begin with Core Patterns (01-05)

**Building complex workflows?** Explore Advanced Patterns (06-10)

**Deploying to production?** Review System Patterns (11-15)

**Optimizing performance?** Check Optimization Patterns (16-19)

**Making strategic decisions?** Consider Strategic Patterns (20-21)

---

_These patterns are designed to be mixed and matched. Most production systems combine multiple patterns to achieve their goals._
