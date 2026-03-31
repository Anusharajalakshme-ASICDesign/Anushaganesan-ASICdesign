## 📁 Cross functional collaborations (STAR Method)
*Post silicon involvement*

<details>
<summary><b>🔍 High-Stakes GLS Debug & ECO </b></summary>

* **Situation:** During the final sign-off phase, SoC-level Gate-Level Simulation (GLS) failed for a critical IP, despite passing all functional RTL verification. The failure was traced to a mismatch between the RTL and the netlist retention behavior.
* **Task:** Led resolution of a critical SoC-level GLS failure and executed ECO across multiple netlist levels and ensured LEC closure under aggressive tapeout timelines.
* **Action:** Identified a systemic gap in UPF specification handling by synthesis, and drove a cross-domain fix spanning RTL, UPF, and netlist implementation.    
* **Result:** Successfully synchronized the RTL, UPF, and Netlist behavior, allowing the SoC to meet its sign-off milestones on schedule. I subsequently solved, prevented recurrence and influenced methodology for future projects.
* **Impact:** **Prevented multi-week tapeout delay** and improved robustness of low-power signoff methodology across subsequent designs. 
* **Takeaway:** Senior leadership is defined by the ability to remain calm under extreme tape-out pressure and provide optimal, "out-of-the-box" solutions. By going above and beyond my defined role to manage the ECO and LEC personally, I ensured the team overcame a critical crisis that could have resulted in a multi-week schedule slip.
</details>

<details>
<summary><b>🛠️ Silicon Reliability & Burn-in Fix </b></summary>

* **Situation:** Silicon failed reliability tests after three days of burn-in due to an unexpected CPU sleep mode during FW inactivity.
* **Task:** Diagnosed silicon reliability failure during burn-in caused by unintended firmware-triggered CPU sleep states under idle conditions.
* **Action:** Drove cross-functional debug across post-silicon validation and firmware teams, identifying a HW/FW interaction gap. Implemented design changes to enforce deterministic hardware behavior and introduced debug visibility mechanisms.
* **Result:** Established validation checks and HW/FW interaction guidelines adopted in subsequent SoCs, ensuring consistent reliability under stress conditions.
* **Impact:** Enabled **100% pass rate** for production silicon and improved robustness of post-silicon validation strategy across multiple projects.
* **Takeaway:** Post-silicon success requires a "big picture" understanding of how firmware and hardware interact under extreme reliability conditions.
</details>

<details>
<summary><b>🔌 USB Downstream Port-Power & Over-Current Sense (OCS) Optimization</b></summary>

* **Situation:** USB downstream ports utilized a shared-pin configuration for Port Power and Over-Current Sense (OCS). The RTL used a 4ms timer to filter OCS events (where a weak zero signaled an over-current event) to ensure valid reporting for power-off sequences.
* **Task:** Resolved post-silicon failure in USB downstream power delivery caused by mismatch between RTL timing assumptions and real analog power ramp behavior.
* **Action:** Identified limitation in existing debounce logic and redesigned power-on sequencing to incorporate hardware-aware timing margins.
* **Result:** Introduced a robust debounce methodology for shared power/sense interfaces, improving reliability across similar mixed-signal designs.
* **Impact:** Ensured stable power delivery across all downstream ports and **influenced design practices** for handling analog-digital boundary conditions.
* **Takeaway:** Post-silicon validation requires a deep understanding of analog electrical characteristics (like power ramp-up) that are often simplified in RTL and Gate-Level Simulations (GLS).
</details>
