
---
name: agent-knowledge
description: Provides knowledge about the organization's active Multica agents, including their objectives, responsibilities, capabilities, skills, dependencies, boundaries, and relationships. Use for agent discovery, capability questions, routing recommendations, and organizational agent analysis.
---

# Agent Knowledge

## Purpose

Provide reliable knowledge about the current Multica agent organization.

## Sources

Read the following reference files:

1. `references/AGENT_REGISTRY.md`
   - Agent identity
   - Objective
   - Responsibilities
   - Capabilities
   - Inputs and outputs
   - Boundaries

2. `references/AGENT_RELATIONSHIPS.yaml`
   - Dependencies
   - Agent relationships
   - Collaboration and handoffs

3. `references/AGENT_AUDIT.md`
   - Overlapping responsibilities
   - Capability gaps
   - Risks and recommendations

## Rules

- Use the registry as the primary source for questions about registered agents.
- Do not invent agent capabilities.
- Distinguish confirmed facts from inferred relationships.
- Explain when the registry was last synchronized.
- Do not assume that a documented capability has been verified by an execution test.
- If information is missing, explicitly state that it is unknown.
- Never modify another agent's configuration.
- Never expose secrets or credentials.

## Response Format

For agent-specific questions, provide:

- Agent name
- Objective
- Capabilities
- Responsibilities
- Inputs
- Outputs
- Dependencies
- Boundaries

For organization-wide questions, provide comparisons, relationships, overlaps, and gaps.

When information may be outdated, recommend running Agent Registry Sync.
