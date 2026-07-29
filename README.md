# 🐉 Ze Ri (Date Selection) AI Quality Control Auditor

An advanced Prompt Engineering & Domain-Specific AI System designed for high-precision Ze Ri (Date Selection) audits under classical Chinese Metaphysics (Joey Yap methodology).

This framework acts as a **Senior Quality Control Auditor**, screening candidate dates against spatial, temporal, personal, and elemental afflictions, and categorizing viable dates into a prioritized client recommendation report.

---

## 🌟 Key Features & Logic Architecture

- **Property-First Hierarchy:** Prioritizes House Sitting directions and subsector 24-Mountain accuracy before personal or daily indicators.
- **Zero-Compromise Hard Eliminations:** Automated detection and removal of fatal afflictions:
  - **Spatial:** Annual & Monthly Three Killings (*San Sha*), Monthly 5 Yellow, 180° Mountain Clashes.
  - **Personal:** Client Year Branch Clashes (*Sui Po*).
  - **Temporal & SOP Red Flags:** Yang Gong Disaster Days, Month Breakers, Destruction (*Po*) / Close (*Bi*) Day Officers.
- **Elemental & Activation Matching:** Enforces Na Yin / Branch elemental harmony for specific events (e.g., Fire Activations, Metal 5-Yellow Remediation).
- **Day Officer Priority Hierarchy:** Strictly reserves Tier 1 and Tier 2 rankings for Primary "Good Days" (*Success, Open, Stable, Initiate, Remove*), demoting secondary conditional days (*Establish, Full, Receive*) to Tier 3.
- **Dynamic Override Engine:** Integrates *Great Sun (Tai Yang)* and *Great Moon (Tai Yin)* formulas to safely neutralize minor annual spatial afflictions.

---

## 📁 Knowledge Base Integration

The system leverages a **RAG-style (Retrieval-Augmented Generation)** knowledge architecture, linking the core prompt engine to modular external guidelines:
1. **`@SOP_Date_Selection_Rules`**: Hard elimination criteria and procedural guidelines.
2. **`@Ze_Ri_Guideline_Document`**: Auxiliary star definitions (Boosters vs. Blockers) and Dong Gong rating charts.
3. **`@24_Mountains_Map`**: Subsector degree mappings and specific animal clash pairs.

---

## 📋 Sample Usage & Inputs

```text
[CLIENT & PROPERTY PARAMETERS]
- Clients: Goat (未), Rat (子), Ox (丑)
- Event: Fire Activation at West Sector
- Property Sitting Direction: North 2 (Rat 子)
- Target Sector: West

[BATCH DATES REVIEWED]
Candidate list of 20+ raw dates across July – December.
```

---

## 📊 Sample Audit Report Output

Check out [`examples/sample_audit_report.md`](./examples/sample_audit_report.md) to see a full output example, including:
- **Internal Rejected Summary:** Explicit reasons for auto-elimination (e.g., *Yang Gong Day*, *Rat Breaker*, *Monthly San Sha*).
- **Client Recommendation List:** Tiered (Tier 1 to Tier 3) recommendations with recommended double-hour slots and client notes.

---

## 🛠️ How to Deploy

1. Open your AI environment (e.g., Gemini / Google Workspace).
2. Attach/tag the knowledge base documents in `docs/`.
3. Copy the system prompt from `prompt_templates/master_audit_prompt.md`.
4. Input client/property parameters and candidate date batch.
