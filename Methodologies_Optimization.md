## 📁 Methodologies Case Studies (STAR Method)
*High-impact stakeholders involvement*

<details>
<summary><b>🚀 CDC/RDC Methodology Optimization </b></summary>

* **Situation:** Traditional CDC analysis tools were insufficient for complex SoC-level verification, often missing critical IP-level constraints.
* **Task:** Lead the transition to **VC SpyGlass** (AI/ML supported) and define a scalable SoC-level flow in absence of standardized IP constraints.
* **Action:** Independently spearheaded the implementation of the VC SpyGlass flow and presented data-driven benchmarks to stakeholders to secure organizational buy-in.
* **Result:** Drove adoption across multiple SoC teams by presenting benchmark data and demonstrating **~30%** improvement in analysis efficiency and reduction in manual triage effort.
* **Impact:** Established a reusable, high-coverage CDC framework that became the **standard baseline for subsequent SoC programs**.
* **Takeaway:** Proactive adoption of advanced EDA capabilities and cross-team standardization is the key to managing the verification complexity of next-generation SoCs.
</details>

<details>
<summary><b>🔍 Critical LEC/UPF Debug & ECO </b></summary>

* **Situation:** "X" propagation issues were discovered in Gate-Level Simulation (GLS), threatening the project timeline.
* **Task:** As the IP Design Lead, I took ownership and led resolution of critical GLS “X” propagation issue by identifying gaps in UPF retention modeling and aligning RTL, UPF, and physical implementation.
* **Action:** Drove architectural decision to replace retention strategy, implemented **ECO** across 6 netlists, and ensured LEC closure under tight tapeout timelines.
* **Result:** Secured **LEC equivalence** in a critical timeframe, ensuring first-pass silicon success.
* **Impact:** **Received formal recognition and applause from upper management** for proactive problem-solving that saved the project schedule.
* **Takeaway:** This intervention prevented schedule slip and reinforced signoff methodology for low-power verification across subsequent designs.

  
</details>

<details>
<summary><b>⚙️ Complex LEC Runtime Optimization </b></summary>

* **Situation:** A critical IP integration faced massive LEC runtime issues (28+ hours), which were deemed a "real challenge" even for tool experts.
* **Task:** Diagnosed LEC convergence bottlenecks during large-scale IP integration by identifying RTL initialization inconsistencies and tool comparison inefficiencies.
* **Action:** Identified a critical RTL bug with default 'X' value instead of '0'; Optimized solver configuration and debug strategy, improving turnaround time and enabling faster iteration during critical integration phases.
* **Result:** Reduced verification time from **~1.5 days to 6 hours**.
* **Impact:** **Applauded by both Synopsys and the SoC project team** Contributed to improved LEC debugging practices for complex designs in collaboration with EDA vendors.
* **Takeaway:** Continuous learning and collaboration with EDA partners are cornerstones of effective problem-solving in advanced digital design.

  
</details>

<details>
<summary><b>⏱️ High-Complexity CDC Sign-off & Noise Reduction (0-in/Mentor Graphics)</b></summary>

* **Situation:** Led CDC signoff for multi-clock SoC (60MHz–125MHz domains), reducing **~100K initial violations to clean signoff** by defining custom synchronizer models and refining clock grouping strategies.
* **Task:** Eliminated false-positive noise and established a repeatable CDC signoff methodology using SDC and behavioral modeling.
* **Action:** * Implemented **Custom Synchronizer** definitions to explicitly map FIFO and pulse-synchronizer behavioral models for tool recognition.
* **Result:** Successfully reduced 100k violations to a clean, verified sign-off state, ensuring stable data transfer across asynchronous boundaries.
* **Impact:** **Established a high-integrity CDC sign-off methodology** Eliminated false-positive noise and established a repeatable CDC signoff methodology using SDC and behavioral modeling.
* **Takeaway:** Effective CDC sign-off is not just about running a tool; it requires a deep understanding of the design's clock architecture and the ability to "teach" the tool to recognize custom synchronization hardware.
</details>
