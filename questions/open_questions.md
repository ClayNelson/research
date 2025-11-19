# Open Questions
_Updated: 2025-11-19_

This file tracks the highest-leverage unanswered questions across the domains of:
- ARM-native compute & multi-architecture evolution  
- Edge AI & hardware–software co-design  
- Agentic systems & MCP-style orchestration  
- Regulated developer experience (automotive, industrial, IoT, healthcare)  
- AI-native organizational design & complexity reduction  

Questions remain open until:
1. A run provides strong evidence (confirming or contradicting)  
2. A world model revision resolves or reframes the question  
3. The question is archived or matured into a hypothesis  

---

## 1. ARM-Native Compute & Multi-Architecture Future

### **1.1 What is the real upper bound of Arm adoption in cloud AI workflows?**
- GPU-dominated clusters reduce CPU architecture importance.  
- Some operators shifting back to x86 for operational simplicity.  
- Open: At what workload mix does Arm meaningfully win vs. cap out?

### **1.2 Will developer continuity (M-series → Arm CI → Cobalt/Graviton) be strong enough to override x86 inertia?**
What evidence would indicate a true phase shift:
- build pipelines defaulting to Arm?  
- Arm-first SaaS vendors?  
- enterprise procurement shifts?  

### **1.3 What is the tipping point for multi-architecture as the norm?**
- Is multi-arch the endgame or a transition state?  
- How fast are Google/AWS/Azure converging on unified pipelines?  

---

## 2. Edge AI & HW/SW Co-Design

### **2.1 How quickly will certifiable reference stacks become standardized?**
- Wind River, QNX, NVIDIA, Siemens — all building vertically.  
- Is fragmentation increasing or consolidating?  
- Who becomes the “Kubernetes of edge safety stacks”?

### **2.2 Can generic edge-AI frameworks ever realistically compete with domain-specific stacks?**
If so, under what conditions:
- universal IR formats?  
- standardized quantization toolchains?  
- next-gen safety certification protocols?  

### **2.3 How does lifecycle/tooling (model mgmt, updates, evidence) become standardized across hardware?**
This is a major open coordination problem.

---

## 3. Agentic Systems & MCP-Style Protocols

### **3.1 Will MCP, A2A, ACP, or a new protocol become the dominant agent interface?**
- Is protocol pluralism permanent?  
- What incentives favor unification vs. fragmentation?

### **3.2 How will enterprises decide the boundaries of agent autonomy?**
Questions include:
- where do agents run (local/cloud/OT)?  
- what guardrails become mandatory?  
- what counts as “certifiable autonomy”?  

### **3.3 What shapes the eventual hierarchy of control planes?**
- GitHub Agent HQ (developer)  
- Azure Foundry Agent Service (enterprise/business)  
- OT/RTOS stacks (safety-critical)  
Is there a predictable equilibrium?

---

## 4. Regulated Developer Experience (Automotive, Industrial, IoT, Healthcare)

### **4.1 What would make GitHub a first-class participant in regulated DevEx?**
Is it:
- safety-case generation?  
- evidence pipelines?  
- integration with RTOS toolchains?  
- certification-grade traceability?  

### **4.2 Will safety-critical industries adopt agentic development sooner or later than cloud/enterprise?**
- Agents might help automate evidence generation.  
- But autonomy risk tolerance is lower.  
Which wins out?

### **4.3 How will domain vendors (Bosch, Siemens, Wind River, QNX) leverage GitHub or bypass it?**
What is the stable interface layer between vertical stacks and GitHub’s horizontal platform?

---

## 5. AI-Native Organizational Design & Complexity Compression

### **5.1 What is the true pacing function for organizational simplification?**
Does simplification follow:
- tool maturity,  
- platform consolidation,  
- leadership culture shift,  
- or regulatory pressure?

### **5.2 Which org archetype wins:**
- **Agent-first**, flat, generalist-heavy?  
- **Platform-first**, tightly constrained?  
- **Hybrid**, with strong governance but flexible execution?

### **5.3 What does “AI-native management” look like in practice?**
Open questions:
- What replaces traditional reporting?  
- How is coordination measured?  
- What skills dominate leadership?  

---

# Meta-Questions

These guide how the entire research system evolves:

### **M1. What are the earliest signals that should trigger a world model revision?**

### **M2. How do we measure “world model accuracy”?**

### **M3. Which open questions should be converted into explicit predictions and bets?**

### **M4. When should we promote an open question → hypothesis → canonical belief?**

---

# Archival Note
Older resolved questions will move to:
`questions/archive.md`
