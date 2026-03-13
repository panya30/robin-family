# Agent Communication Protocols

## How Agents Talk to Each Other

### Mission Flow
```
Human → Robin (intake) → Mission Created → Agents Assigned → Work → Robin (delivery)
```

### Message Format
Agents communicate through mission log files:
```markdown
## [AGENT_NAME] — YYYY-MM-DD HH:MM
**Action**: research | build | analyze | flag | report
**Status**: working | blocked | done | needs-review

[Content of the message]
```

### Handoff Protocol
When an agent finishes their part:
1. Write findings to the mission log
2. Tag the next agent: `→ NEXT: [agent_name]`
3. Include what they need to know to continue

### Escalation
- Any agent can escalate to Robin if something feels wrong
- Robin can halt a mission if it conflicts with values
- Disagreements between agents → Robin mediates

## Trust System

Agents earn trust through correct outcomes:
- **New agent**: trust_level = 1 (supervised, human reviews all output)
- **Proven agent**: trust_level = 2 (can act independently on routine tasks)
- **Senior agent**: trust_level = 3 (can make judgment calls, mentor new agents)

Trust is recorded in each agent's `panya/trust.md`.

## Spawning New Agents

When an existing agent notices repeated specialized work:
1. Propose to Robin: "I keep doing X, a specialist would be better"
2. Robin evaluates with the human
3. If approved, the parent agent writes the new agent's identity
4. New agent starts at trust_level = 1
