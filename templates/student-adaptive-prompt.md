Act as an AP Chemistry Master Teacher, Science of Learning Specialist, and Lead EdTech Web Developer. Create a single, standalone, zero-dependency HTML file (containing HTML, embedded CSS in <style> tags, and embedded JavaScript in <script> tags) for an "Interactive Multi-Representational Student Lab Companion."

### TECHNICAL GUARANTEES:
1. Deliver the output as a single, 100% complete HTML file. Do NOT truncate code, omit functions, or use comment placeholders like "// rest of code here".
2. Use plain-text formatting for all chemical formulas, units, and math equations (e.g., write "H2O2", "KMnO4", or "M1V1 = M2V2"). Do NOT output standard LaTeX math delimiters (like $ or $$) that break web rendering.
3. Embed Chart.js via CDN for dynamic graphing. Include a complete, built-in "Export My Work" JavaScript engine that lets students download their responses as an HTML or Markdown file.

---

### CORE PEDAGOGICAL GOAL:
Explicitly help students bridge the gap between Physical Observations (color changes, gas evolution), Live Data Tables, Dynamic Graphs, Particle-Level Reactions (sub-microscopic electron transfer/molecular models), Mathematical Equations (mole ratios/stoichiometry), and Real-World Applications.

---

### UI & ADAPTIVE ARCHITECTURE REQUIREMENTS:

1. DUAL WORKSPACE LAYOUT:
   - Left Panel: Interactive Multi-Representational Simulation & Dynamic Visual Hub.
   - Right Panel: Guided Student Notebook, Inquiry Scaffolding & Export Engine.
   - Top Control Bar: 
     * Student Cognitive Level Selector: [ Level 1: Guided Inquiry (Heavy CER stems, dimensional analysis hints) | Level 2: Standard Inquiry | Level 3: Advanced Challenge (Minimal hints, error derivations) ].
     * Phase Progress Tabs: [ 1. PRE-LAB PLANNING | 2. STATION LAB DAY | 3. POST-LAB REFLECTION & CAREERS ].
     * Button: "Export My Work" (Triggers instant download of student responses).

2. SYNCHRONIZED MULTI-REPRESENTATIONAL SYSTEM (Left Panel):
   Build an interactive HTML5 Canvas/SVG + Chart.js dashboard containing 4 dynamically synchronized modules that update in real-time as students manipulate inputs or sliders:
   - Module A (Physical Visual): Dynamic rendering showing liquid color, phase change, or gas evolution based on experimental progress.
   - Module B (Particle-Level Explorer): Interactive sub-microscopic diagram illustrating ion movement, bond breaking/forming, or electron transfer.
   - Module C (Live Data Table & Dynamic Graph): Live data logging table connected to a real-time line graph plotting experimental variables.
   - Module D (Math & Equation Linker): Live stoichiometric conversion equation mapping raw inputs directly to mole ratios and chemical formulas.

3. RIGHT PANEL: GUIDED STUDENT WORKSPACE:
   - Phase 1 (Pre-Lab): Central challenge breakdown, interactive pre-lab guiding questions with Socratic hint toggles, safety checkboxes, and pre-lab self-audit gate.
   - Phase 2 (Station Work): Chunked procedural workflow, live data logging with sig-fig/precision alerts, Emergent Bilingual (EB) CER sentence stems, and troubleshooting guides.
   - Phase 3 (Post-Lab): Guided calculation & dimensional analysis builder, Claim-Evidence-Reasoning (CER) conclusion builder, and real-world STEM career connection module.

4. EXPORT ENGINE:
   - Collects student name, cognitive level, station data tables, CER responses, and reflection answers into a beautifully formatted document download for student turn-in.

---

### INSTRUCTIONS FOR GENAI:
Ingest the provided Student Edition lab text, build the synchronized multi-representational modules, and output the complete single-file HTML code block.
