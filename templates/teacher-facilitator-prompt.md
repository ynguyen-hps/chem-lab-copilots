Act as a Lead EdTech Web Developer and Master Science Instructional Coach. Create a single, standalone, zero-dependency HTML file (containing HTML, embedded CSS in <style> tags, and embedded JavaScript in <script> tags) for a high school chemistry "Lab Facilitation & Execution Dashboard."

### TECHNICAL GUARANTEES:
1. Deliver the output as a single, 100% complete HTML file. Do NOT truncate code, omit functions, or use comment placeholders like "// rest of code here".
2. Use plain-text formatting for all chemical formulas, units, and math equations (e.g., write "H2O2", "KMnO4", or "M1V1 = M2V2"). Do NOT output standard LaTeX math delimiters (like $ or $$) that break standard web rendering.
3. Clean, high-contrast UI optimized for laptop screens, tablets, and smartboard/projector displays.

---

### CORE DESIGN PHILOSOPHY:
Eliminate teacher cognitive overload by splitting the dashboard into two clean focus areas:
1. TAB 1: GENERAL LAB PREP & OVERVIEW (The 1-Page Planning Snapshot)
2. TAB 2: LIVE IN-CLASS FACILITATOR (The Daily 3-Phase Interactive Dashboard)

---

### UI & DASHBOARD ARCHITECTURE:

1. TOP CONFIGURATION BAR:
   - Select Lab / Activity (Populated from the provided curriculum/lab data).
   - Total Student Count & Available Lab Stations Count.
   - Lab Duration Selector (Select 1 to 5 Days).
   - Track Toggle (On-Level vs. Honors vs. AP).

2. TAB 1: GENERAL LAB PREP & OVERVIEW (Before Day 1)
   - Purpose & Learning Goals: Core TEKS/standards, big ideas, and central inquiry challenge.
   - Dynamic Station Supply Scaler: Auto-calculates total chemicals, equipment, and glassware needed based on Student & Station counts.
   - Grouping & Lab Roles: Automatic breakdown of student group sizes and assigned student roles (e.g., Materials Manager, Safety Lead, Data Collector).
   - Master Safety & Waste Protocol: Goggles, SDS protocols, chemical handling, and disposal/neutralization steps.

3. TAB 2: LIVE IN-CLASS FACILITATOR (During Lab Days)
   - Phase Selector: Switch between [ PRE-LAB DAY | LAB DAY(S) | POST-LAB DAY ].
   - Multi-Day Selector: Tabs for Day 1, Day 2, Day 3, etc., based on chosen lab length.
   - Daily Classroom Routine Blocks (For each active day):
     * BLOCK 1: DO NOW / PRIOR KNOWLEDGE (5–10 Mins)
       - Board-ready warm-up question reviewing prior day concepts or key safety checks.
     * BLOCK 2: EXPLORE & EXPLAIN (Main Class Period)
       - Live Countdown Timer with 30-second TLAC transition alerts ("Tight Transitions").
       - Visible Thinking & Discussion Prompts: Targeted Socratic questions to drive student dialogue during active station work.
       - Teacher "Radar" Walkthrough Checklist: Timed monitoring alerts for safety, measurement accuracy, and data collection.
       - Embedded Student Scaffolds: Emergent Bilingual (EB) sentence stems and SPED chunked instructions.
     * BLOCK 3: CLEAN-UP & DAILY TAKEAWAYS (Last 5 Mins)
       - Dedicated 5-minute clean-up countdown timer.
       - Daily exit ticket / quick CFU prompt to synthesize the day's observations before leaving.

4. PROJECTOR / BOARD FULL-SCREEN MODE:
   - A single-click "Project to Board" button that launches a high-contrast, clutter-free modal display for the smartboard showing ONLY:
     * Active Stage Timer (Do Now, Lab Work, or Clean-up).
     * Visible Thinking Stems & Discussion Prompts for students.
     * Projected Data Collection Tables / Clean-up instructions.

5. POST-LAB MODULE (Data Analysis & Reflection):
   - Data Synthesis Guide: Class-wide data pooling template.
   - Graphical & Mathematical CFU Prompts: Step-by-step guidance for error analysis, percent error calculation, and Claim-Evidence-Reasoning (CER) conclusions.
   - Final Packet Completion Checklist: Final review checklist to help students complete their lab packets.

---

### INSTRUCTIONS FOR GENAI:
Ingest the provided curriculum/lab text, extract all procedural steps, safety notes, supplies, and questions, and output the complete, fully functional single-file HTML code block.
