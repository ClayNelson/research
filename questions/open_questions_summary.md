# Open Questions Summary
_Generated: 2025-11-19_

This document provides a **synthesized view** of the open research questions tracked in `open_questions.md`, organized by strategic priority and readiness for hypothesis promotion.

---

## Executive Summary

The repository currently tracks **20 domain questions** across 5 research areas, plus **4 meta-questions** about the research system itself. 

**Key findings:**
- **7 questions** are ready for hypothesis promotion based on recent evidence
- **5 questions** represent the highest strategic leverage for near-term focus
- **3 cross-cutting themes** link multiple questions across domains
- **4 questions** may need reframing or archival

---

## I. Questions Ready for Hypothesis Promotion

These questions have accumulated sufficient evidence from recent scans to warrant promoting to explicit hypotheses:

### **1.1 → ARM adoption upper bound (Question 1.1)**
**Recent evidence:**
- GitHub Arm64 runners + Azure Cobalt GA demonstrate ecosystem continuity
- Python Software Foundation migration validates mainstream feasibility
- BUT: QNX pairing with Intel/Nvidia, GPU-heavy clusters staying x86

**Suggested hypothesis:**  
*"Arm wins as the preferential default for new cloud-native and edge AI workloads over the next 3-5 years, while x86 + GPU remain entrenched for legacy and heavy training. Multi-arch tooling becomes the norm."*

### **1.2 → Developer continuity as phase shift signal (Question 1.2)**
**Recent evidence:**
- Arm migration assistant for GitHub Copilot
- Windows Arm64 runners
- M-series → CI → cloud path solidifying

**Suggested hypothesis:**  
*"Developer continuity (M-series → Arm CI → Cobalt/Graviton) creates sufficient gravity for Arm to become the 'optimized default' without triggering wholesale x86 displacement. The phase shift is continuity preference, not performance dominance."*

### **2.1 → Certifiable reference stacks consolidation (Question 2.1)**
**Recent evidence:**
- Wind River, QNX, NVIDIA, Siemens all building vertically integrated stacks
- No signs of consolidation; fragmentation increasing

**Suggested hypothesis:**  
*"Certifiable edge stacks will remain fragmented across vendors (Wind River, QNX, Siemens) for 5+ years. The 'Kubernetes of edge safety' won't emerge; instead, vertical integration will deepen, creating a heterogeneous multi-stack reality."*

### **3.1 → Agent protocol dominance (Question 3.1)**
**Recent evidence:**
- MCP solidifying as default but explicitly vendor-neutral
- Multiple agent frameworks wrapping MCP
- GitHub positioned as "one MCP server among many"

**Suggested hypothesis:**  
*"MCP becomes the lingua franca for agent-tool communication, but protocol pluralism remains permanent at the control plane level. No single protocol 'wins'—instead, interop layers emerge."*

### **3.3 → Agent control plane hierarchy (Question 3.3)**
**Recent evidence:**
- GitHub Agent HQ (developer)
- Azure AI Foundry Agent Service (enterprise)
- OT/RTOS stacks (safety-critical)
- Clear vertical-horizontal tensions

**Suggested hypothesis:**  
*"Agent control planes will be federated and vertical-specific: GitHub as dev HQ, Azure Foundry as enterprise HQ, OT systems (Industrial Edge, Wind River Studio) as safety HQ. The equilibrium is polycentric, not unified."*

### **4.1 → GitHub in regulated DevEx (Question 4.1)**
**Recent evidence:**
- Partnership on AI report on runtime monitoring
- Black Duck on AI-code compliance
- Wind River/QNX emphasizing evidence pipelines

**Suggested hypothesis:**  
*"GitHub becomes a first-class participant in regulated DevEx by enabling 'evidence-generating development systems'—automated SBOM generation, safety case artifacts, traceability pipelines—positioned as the code cortex, not the operational brain."*

### **5.1 → Organizational simplification pacing (Question 5.1)**
**Recent evidence:**
- Consulting literature shows AI layers added on top of existing structures
- No evidence of radical downsizing yet
- Complexity increasing in near term

**Suggested hypothesis:**  
*"AI-native organizational simplification is paced by platform consolidation, not tool maturity. Complexity increases for 3-5 years as companies add AI layers, governance, and agent platforms; simplification only follows platform hardening."*

---

## II. Highest-Leverage Questions for Near-Term Focus

These questions have the most strategic impact and are underserved by current research:

### **Priority 1: Vertical–Horizontal Interface Layer (NEW)**
**Why it matters:**  
The interface between vertical safety stacks (RTOS, toolchains) and horizontal platforms (GitHub, Azure) is where economic and political power is negotiated. This is not explicitly called out in current questions but emerges as critical.

**Suggested new question:**  
*"What becomes the stable interface layer between vertical stacks (Wind River, QNX, Siemens) and horizontal platforms (GitHub, Azure), and who controls it?"*

### **Priority 2: Evidence-Generation as First-Class Asset (4.1 reframed)**
**Why it matters:**  
Regulated DevEx is not about faster CI/CD—it's about automated compliance artifact generation. This reframing changes the value proposition entirely.

**Suggested reframe of 4.1:**  
*"What evidence-generation primitives (SBOM, safety cases, runtime monitoring logs, AI-code provenance) become standardized across GitHub and OT platforms, and how do they compose?"*

### **Priority 3: Edge AI Closed-Loop Reliability vs. Full Autonomy (2.2 reframed)**
**Why it matters:**  
The real near-term value of edge AI is human-in-the-loop reliability (predictive maintenance, quality inspection), not fully autonomous control loops.

**Suggested reframe of 2.2:**  
*"What is the ROI curve for edge AI closed-loop reliability systems vs. fully autonomous safety-critical control, and where does certification risk cap out autonomous adoption?"*

### **Priority 4: Agent Primitives for Safety-Critical Domains (NEW)**
**Why it matters:**  
Regulated domains will require new agent capabilities: provenance-aware agents, evidence-generating agents, bounded autonomy agents, certifiable toolchain agents. These are a future competitive surface.

**Suggested new question:**  
*"What agent primitives emerge as 'must-haves' for regulated domains, and which vendors/platforms build them first?"*

### **Priority 5: Multi-Arch as Steady State (1.3 reframed)**
**Why it matters:**  
The question currently asks if multi-arch is the norm or a transition state. Recent evidence strongly suggests it's the steady state—but this needs to be formalized.

**Suggested reframe of 1.3:**  
*"How do toolchains, CI/CD platforms, and developer workflows evolve to treat multi-arch (Arm + x86 + GPU) as the default, not the exception—and what does 'good' multi-arch DevEx look like?"*

---

## III. Cross-Cutting Themes

These themes link multiple questions across domains:

### **Theme A: Verticalization vs. Platformization Tension**
**Affects questions:** 2.1, 2.2, 3.3, 4.3  
**Insight:** Regulated and edge domains are verticalizing (Wind River, QNX, Siemens, Bosch) while developer domains are platformizing (GitHub, Azure). The stable interface layer between these is the key leverage point.

### **Theme B: Complexity Spike Before Simplification**
**Affects questions:** 2.3, 5.1, 5.2, 5.3  
**Insight:** AI-native systems increase complexity in the near term (more platforms, more governance, more monitoring) before simplifying. The pacing function is platform consolidation, not tool maturity.

### **Theme C: Federated Control as Structural Outcome**
**Affects questions:** 3.1, 3.2, 3.3, 4.3  
**Insight:** Agent control planes will be polycentric and domain-specific (dev, enterprise, OT), not unified. MCP provides interop, but control remains federated. This is now a structural inevitability, not a strategic choice.

---

## IV. Questions Needing Reframing or Archival

### **4.2 → Safety-critical agentic adoption timing**
**Current state:** Asks whether safety-critical industries adopt agents sooner or later than cloud/enterprise.

**Issue:** This is binary and may be unanswerable without more data. Recent evidence (Bosch, Siemens) shows they're adopting *differently* (evidence-generation focus, human-in-loop), not just earlier/later.

**Suggested action:** Reframe as: *"How do agent adoption patterns differ between cloud/enterprise (productivity, autonomy) and safety-critical (evidence-generation, human-in-loop) domains, and what does this imply for platform design?"*

### **5.2 → Winning org archetype**
**Current state:** Asks which archetype wins: agent-first flat, platform-first constrained, or hybrid.

**Issue:** Recent evidence suggests the answer is "hybrid" by default—companies add AI layers atop existing structures. This question may be too abstract.

**Suggested action:** Archive or reframe as: *"What does the 'agent-first hybrid' organization look like in practice—what layers remain, what layers dissolve, and what new coordination mechanisms emerge?"*

### **M3 → Converting questions to predictions**
**Current state:** Meta-question about which questions become predictions and bets.

**Issue:** This is already answered by this document—questions with sufficient evidence (Section I) should become predictions.

**Suggested action:** Archive M3 and replace with: *"What is the right cadence for promoting questions → hypotheses → canonical beliefs, and how do we avoid premature commitment?"*

### **M4 → Promotion criteria**
**Current state:** Asks when to promote questions to hypotheses to beliefs.

**Issue:** Similar to M3—this document provides the answer.

**Suggested action:** Archive M4 and replace with: *"How do we measure confidence in canonical beliefs, and when should we demote them back to hypotheses?"*

---

## V. Recommended Next Actions

Based on this summary, here are concrete next steps:

### **Immediate (next scan):**
1. Promote 7 questions from Section I to explicit hypotheses
2. Add 2 new questions from Priority list (vertical-horizontal interface, agent primitives)
3. Reframe 3 questions (4.2, 5.2, and one from Priority list)
4. Archive or revise 2 meta-questions (M3, M4)

### **Short-term (next month):**
1. Design mini-experiments to test Priority 2 (evidence-generation primitives)
2. Conduct targeted research on Priority 1 (vertical-horizontal interface layer)
3. Create a "hypothesis tracker" to monitor confidence levels in promoted questions

### **Ongoing:**
1. Use this summary format after each twice-weekly scan
2. Update cross-cutting themes as new patterns emerge
3. Track which hypotheses get confirmed/refuted by subsequent scans

---

## VI. Quality Metrics for Open Questions

To maintain high signal-to-noise ratio, questions should meet these criteria:

### **Good question characteristics:**
- **Testable:** Can be answered with observable evidence
- **Strategic:** Affects decision-making or resource allocation
- **Specific:** Avoids vague language or multiple sub-questions
- **Timely:** Relevant to current or near-term market state

### **Questions to archive:**
- Already answered by recent evidence
- Too abstract to guide action
- Conflated with other questions
- No longer strategically relevant

### **Questions to refine:**
- Multiple questions bundled into one
- Binary when the answer is "both/and"
- Missing context or framing
- Unclear success criteria

---

## VII. Appendix: Full Question Inventory

For reference, here's the complete list of 24 questions currently tracked:

**ARM-Native Compute (3):**
1.1, 1.2, 1.3

**Edge AI & HW/SW Co-Design (3):**
2.1, 2.2, 2.3

**Agentic Systems & MCP (3):**
3.1, 3.2, 3.3

**Regulated Developer Experience (3):**
4.1, 4.2, 4.3

**AI-Native Org Design (3):**
5.1, 5.2, 5.3

**Meta-Questions (4):**
M1, M2, M3, M4

**Total:** 20 domain questions + 4 meta-questions = **24 open questions**

**Recommendations:**
- Promote: 7 questions → hypotheses
- Add: 2 new questions
- Reframe: 3 questions
- Archive: 2 questions

**Net change:** +0 questions (7 promoted, 2 archived, 2 added, 3 reframed)

---

_End of summary. Next review: After 2025-11-21 scan._
