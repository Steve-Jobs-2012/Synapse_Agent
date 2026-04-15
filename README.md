# Synapse_Agent

A privacy-first, locally-deployed intelligent personal assistant based on Kimi K2.5, featuring dynamic expert routing, hierarchical memory architecture, and secure multi-agent collaboration.

---

## Core Features

### 1. Model Architecture Optimization

| Optimization | Description |
|-------------|-------------|
| **Mode Fusion** | Merges Thinking + Agent modes, eliminates Instant mode |
| **Dynamic Expert Routing** | Evaluates task complexity at k=8, then dynamically adjusts k (2/4/8/16/32/64/128) |
| **Adapter Stacking** | Independent capability modules, fused with SVD compression |
| **INT4 Quantization** | Reduces VRAM to ~180GB, consumer-grade hardware compatible |

### 2. Memory & Context Management

- **20 Memory Spaces**: Episodic, semantic, procedural, reminders, etc.
- **Dual-Layer Context**: Full context (compressed storage) + Fast-access layer (dynamic summaries)
- **KV Cache Isolation**: Physical separation between main agent and sub-agents
- **Message Bus**: Queue-based scheduling for parallel multi-tasking

### 3. Security Architecture (Improvements over OpenClaw)

| Risk Vector | OpenClaw Status | Synapse_Agent Solution |
|-------------|-----------------|------------------------|
| **Command Injection** | Agent may execute malicious commands (`rm -rf /`) | **Whitelist**: Predefined safe commands only |
| **Email/Message Hijacking** | Misled agent sends messages to attackers | **Double Confirmation**: Sensitive ops require explicit user approval |
| **Privacy Data Leakage** | Memory may be tricked into revealing info | **Tiered Permissions**: Sensitive spaces require additional auth |
| **Sub-Agent Privilege Escalation** | Sub-agents may access all memory | **Restricted Sandbox**: Sub-agents access designated spaces only |
| **Network Attack Surface** | Default open MCP tools | **Local-First**: Local APIs preferred, network ops require toggle |

### 4. Multi-Agent Collaboration

