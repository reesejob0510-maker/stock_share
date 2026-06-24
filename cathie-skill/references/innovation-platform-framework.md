# Innovation Platform Framework

Use this file when mapping a technology theme to ARK's five innovation platforms and identifying the disruption logic.

> ARK Invest identifies five major innovation platforms converging simultaneously. Each platform follows a Wright's Law cost curve. When platforms converge, the disruption is multiplicative — autonomous vehicles require AI, energy storage, and robotics simultaneously.

---

## The Five Innovation Platforms

### Platform 1 — Artificial Intelligence

**Core disruption**: Software that learns replaces rule-based software and, increasingly, human cognitive labor.

**Disruption target**: Knowledge work, data analysis, software development, content creation, customer service, medical diagnosis, drug discovery.

**Key cost driver**: Training compute cost follows a ~2.5× improvement per year (inference cost declines even faster). As cost falls, AI becomes embedded in every software application.

**S-curve status (as of 2024–2026)**: Early majority. LLM adoption crossing the chasm in enterprise software; agentic AI beginning Early Adopter phase.

**Key inflection thresholds**:
- LLM API cost below $1/million tokens → enables mass-market consumer applications (crossed ~2024).
- AI agent reliability above 95% on complex tasks → enables autonomous workflow replacement.
- Multimodal AI cost parity with human professional → enables knowledge worker displacement at scale.

**Key layers**:
- Foundation model developers (training compute, model IP)
- Inference infrastructure (GPU clusters, edge silicon)
- Platform / API layer (developer access, fine-tuning)
- Vertical application layer (healthcare AI, legal AI, coding AI)

**Disrupted incumbents**: Traditional enterprise software (ERP, CRM without AI integration), BPO/outsourcing, entry-level knowledge work.

---

### Platform 2 — Autonomous Mobility

**Core disruption**: Self-driving software + electric powertrains replace human-driven, fossil-fuel vehicles.

**Disruption target**: Personal vehicle ownership, taxi/rideshare labor cost, trucking, urban logistics, public transit.

**Key cost drivers**:
- Battery cost (Wright's Law ~18% per doubling; current ~$100/kWh, target <$60/kWh for grid parity).
- LiDAR / sensor cost (from $75,000 in 2012 to <$500 in 2024; target <$100 for mass deployment).
- Compute cost for inference at the edge.

**S-curve status**: Varies by segment.
- Consumer EV: Early Majority in China, Crossing Chasm in US/Europe.
- Autonomous robo-taxi: Early Adopter (Waymo in select US cities).
- Autonomous long-haul trucking: Lab/Early Adopter.

**Key inflection thresholds**:
- Battery cost < $60/kWh → grid storage economic; EV total cost of ownership below ICE in all segments.
- Robo-taxi cost per mile < $0.50 → cheaper than personal car ownership, triggering ownership model shift.

**Disrupted incumbents**: ICE automakers, oil & gas (transportation demand), auto insurance (accident rates decline).

---

### Platform 3 — Robotics

**Core disruption**: General-purpose robots replace human physical labor across manufacturing, logistics, and services.

**Disruption target**: Warehouse labor, factory assembly, last-mile delivery, food preparation, elder care, surgery.

**Key cost drivers**:
- Actuator cost (precision reducers, motors, encoders): dominated by learning-rate improvements in manufacturing scale.
- Compute for real-time motion planning: declining with AI inference cost.
- Vision and tactile sensing: improving with camera and sensor learning rates.

**S-curve status**: Early Adopter for industrial robotics; Lab/Early Adopter for humanoid robots.

**Key inflection thresholds**:
- Humanoid robot cost < $20,000 → competitive with average US manufacturing labor cost per year.
- General manipulation task success rate > 99% → enables flexible deployment without reprogramming.

**Disrupted incumbents**: Low-wage manufacturing regions, warehouse staffing agencies, some surgical device incumbents.

---

### Platform 4 — Energy Storage

**Core disruption**: Cheap, scalable batteries enable intermittent renewable energy to replace fossil fuel baseload and transform transportation.

**Disruption target**: Natural gas peaker plants, coal baseload, ICE vehicles, grid infrastructure (unidirectional → bidirectional).

**Key cost driver**: Battery cell cost. Wright's Law learning rate ~18% per doubling of cumulative production.
- 2010: ~$1,100/kWh
- 2023: ~$100/kWh
- Target: ~$60/kWh (grid storage economic); ~$40/kWh (widespread V2G viable)

**S-curve status**: Crossing Chasm for utility-scale storage in high-renewable grids; Early Adopter for V2G / bidirectional charging.

**Key inflection thresholds**:
- Battery < $60/kWh → grid-scale storage cheaper than gas peaker plants in most markets.
- Battery < $40/kWh → bidirectional EV batteries replace home storage; V2G economics work.

**Disrupted incumbents**: Natural gas peaker operators, diesel generator manufacturers, traditional grid management systems.

---

### Platform 5 — Multiomic / Genomic Sequencing

**Core disruption**: Cheap, fast DNA/RNA/protein analysis transforms drug discovery, diagnostics, and personalized medicine.

**Disruption target**: Traditional diagnostics (blood tests, biopsies), drug development timelines, oncology treatment, population health screening.

**Key cost driver**: Sequencing cost per genome. Fastest Wright's Law in history (~40% per doubling).
- 2001: ~$100M per genome (Human Genome Project)
- 2023: ~$200 per genome
- Target: ~$10 per genome → population-scale screening economically viable; liquid biopsy as routine annual test.

**S-curve status**: Crossing Chasm for oncology genomics; Early Majority for NIPT/prenatal screening; Lab for mRNA therapeutic platforms.

**Key inflection thresholds**:
- Sequencing cost < $10/genome → routine annual cancer screening viable; enables multi-cancer early detection at scale.
- mRNA platform cost parity with small molecule → enables personalized cancer vaccines at scale.

**Disrupted incumbents**: Traditional diagnostic labs (Quest, LabCorp), legacy oncology treatment protocols, some pharmaceutical R&D models.

---

## Platform Convergence — The Multiplier Effect

When two or more platforms converge, the disruption surface expands:

| Convergence | Combined disruption |
|---|---|
| AI + Robotics | General-purpose humanoid robots; autonomous factories |
| AI + Genomics | Protein folding (AlphaFold), AI-designed drugs, digital biology |
| AI + Autonomous Mobility | Full self-driving software; intelligent logistics networks |
| Energy Storage + AI | Smart grid optimization; AI-managed V2G networks |
| Robotics + Energy Storage | Autonomous logistics powered by renewable energy |

**Key insight**: Companies building at the intersection of two or more platforms often have the largest TAM and the strongest network-effect moat. Look for "picks and shovels" that benefit from all platform adoptions.

---

## Innovation Layer Classification (quick reference)

For any company in an innovation theme, assign one of:

| Classification | Description | Example |
|---|---|---|
| **Owns the cost curve** | Deepest learning-rate advantage; costs decline fastest; highest TAM capture | Tesla (battery + EV manufacturing), Illumina (sequencing) |
| **Platform at convergence** | Infrastructure used by all applications built on the technology | NVIDIA (AI compute), AWS (cloud foundation) |
| **First mover in a new use case** | Exploiting a use case unlocked by a recent cost threshold | Exact Sciences (multi-cancer screening after cost cross) |
| **Exposed but not positioned** | In the right sector but without the technology or business model | Legacy auto OEMs with slow EV transition |
| **Disrupted incumbent** | Losing market share to the platform technology | Kodak-equivalent: exposed to full disruption |
