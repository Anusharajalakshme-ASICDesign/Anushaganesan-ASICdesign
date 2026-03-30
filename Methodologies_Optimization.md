## 📁 Methodologies Case Studies (STAR Method)
*High-impact stakeholders involvement*

<details>
<summary><b>🚀 CDC/RDC Methodology Optimization </b></summary>

* **Situation:** Traditional CDC analysis tools were insufficient for complex SoC-level verification, often missing critical IP-level constraints.
* **Task:** Lead the transition to **VC SpyGlass** (AI/ML supported) and implemented a robust SoC-level flow without existing IP constraints.
* **Action:** Independently spearheaded the implementation of the VC SpyGlass flow and presented data-driven benchmarks to stakeholders to secure organizational buy-in.
* **Result:** Improved design analysis efficiency by **30%** and established a standardized CDC flow now utilized across multiple SoC teams.
* **Impact:** **Successfully established a high-coverage verification baseline** that is now the blueprint for other SoC teams within the firm, ensuring scalable growth.
* **Takeaway:** Proactive adoption of advanced EDA capabilities and cross-team standardization is the key to managing the verification complexity of next-generation SoCs.
</details>

<details>
<summary><b>🔍 Critical LEC/UPF Debug & ECO </b></summary>

* **Situation:** "X" propagation issues were discovered in Gate-Level Simulation (GLS), threatening the project timeline.
* **Task:** As the IP Design Lead, I took ownership of the design fix, UPF updates, and proving Logical Equivalence (LEC).
* **Action:** Identified that UPF constraints failed to recognize flop retention behavior; collaborated with the Architect to switch to non-retention flops and implemented the ECO across 6 netlists.
* **Result:** Secured **LEC equivalence** in a critical timeframe, ensuring first-pass silicon success.
* **Impact:** **Received formal recognition and applause from upper management** for proactive problem-solving that saved the project schedule.
* **Takeaway:** Deep technical ownership and the ability to bridge the gap between RTL, UPF, and Physical Design are critical for resolving high-stakes sign-off bottlenecks.
</details>

<details>
<summary><b>⚙️ Complex LEC Runtime Optimization </b></summary>

* **Situation:** A critical IP integration faced massive LEC runtime issues (8+ hours), which were deemed a "real challenge" even for tool experts.
* **Task:** Reduce verification turnaround time and resolve tool performance bottlenecks using alternate solvers.
* **Action:** Debugged and identified a critical RTL vector assigned a default 'X' value instead of '0'; customized tool settings to debug the comparison points more effectively.
* **Result:** Reduced verification time from 8 hours to **6 hours**.
* **Impact:** **Applauded by both Synopsys and the SoC project team** for identifying a tool-level resolution to a complex integration roadblock.
* **Takeaway:** Continuous learning and collaboration with EDA partners are cornerstones of effective problem-solving in advanced digital design.
</details>

<details>
<summary><b>⏱️ High-Complexity CDC Sign-off & Noise Reduction (0-in/Mentor Graphics)</b></summary>

* **Situation:** Using Mentor Graphics 0-in for CDC sign-off on a multi-protocol SoC involving CPU (60MHz), USB2 (60MHz), and USB3 (125MHz) domains. Initial tool runs reported over **100,000 violations**, primarily due to unrecognized synchronization logic and clock grouping issues.
* **Task:** Reduce noise, identify genuine asynchronous hazards, and establish a repeatable, high-confidence CDC sign-off flow using SDC inputs and behavioral models.
* **Action:** * Implemented **Custom Synchronizer** definitions to explicitly map FIFO and pulse-synchronizer behavioral models for tool recognition.
* **Result:** Successfully reduced 100k violations to a clean, verified sign-off state, ensuring stable data transfer across asynchronous boundaries.
* **Impact:** **Established a high-integrity CDC sign-off methodology** that eliminated manual review overhead and guaranteed the reliability of high-speed USB3-to-CPU data paths.
* **Takeaway:** Effective CDC sign-off is not just about running a tool; it requires a deep understanding of the design's clock architecture and the ability to "teach" the tool to recognize custom synchronization hardware.
</details>
