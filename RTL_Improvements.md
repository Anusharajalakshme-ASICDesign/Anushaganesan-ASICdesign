## 📁 Front end Design Case Studies (STAR Method)
*High-impact technical challenges and leadership outcomes:*

<details>
<summary><b>⚡ Architecting Modular, Reusable SoC Design Flows </b></summary>

* **Situation:** A high-performance PSoC family required extreme power efficiency and integration flexibility to support real-time IoT and machine learning applications. The existing subsystem was monolithic, hindering reusability and slowing derivative SoC development.
* **Task:** Led the design and PPA optimization for a high-performance subsystem by restructuring **10 monolithic modules into modular, power-aware IP blocks with independent power domains**. I served as **IP lead for few of the refactored units** and **designed one IP from scratch**, establishing modular UPF flows, timing constraints, and verification standards.
* **Action:** Introduced scalable low-power and modular design practices that enabled dynamic configurability and streamlined integration.
* **Result:** Achieved a **20% reduction in dynamic power**. Delivered a **~60% improvement in design reusability**. The modular design framework has been applied across multiple derivative SoCs, **accelerating development cycles** and enabling faster first-pass silicon success.
* **Impact:** Established a reusable low-power design and integration methodology adopted across **several SoC families**, improving both power-performance-area (PPA) efficiency and organizational scalability.
* **Takeaway:** Strategic modularization of RTL not only achieves immediate PPA targets but creates a **long-term design-for-reusability framework**, demonstrating technical leadership, innovation in methodology, and the ability to influence stakeholders to adopt transformative solutions.
</details>

<details>
<summary><b>🔐 Secure Boot OTP Memory Optimization </b></summary>

* **Situation:** The One-Time Programmable (OTP) was inefficiently re-reading entire regions every time firmware (FW) initiated operations after power-up, causing significant latency.
* **Task:** Redesigned OTP access architecture to eliminate redundant memory reads during firmware initialization by introducing a hardware-controlled state machine for secure data latching.
* **Action:** Orchestrated the hardware state machine to implement a status check at a specific memory location. This triggered a single-run read sequence to latch values locally before handing control to the software.
* **Result:** Improved interaction between hardware and firmware by **offloading repeated** operations and enforcing hardware-level data protection.
* **Impact:** **Reduced boot latency** and established a more efficient HW/FW interaction model for secure memory handling, influencing design patterns for subsequent secure subsystems.
* **Takeaway:** Implementing hardware-level control is a critical structural solution for optimizing the interaction between firmware and secure hardware resources.
</details>

<details>
<summary><b>🚦 Multi-Master Bus Arbitration Priority Optimization </b></summary>

* **Situation:** During high-concurrency multitasking, a collision occurred between two bus masters while writing to a slave's FIFO via DMA. 
* **Task:** Resolved system-level deadlock in multi-master bus architecture by replacing fixed-priority arbitration with a programmable priority mechanism.
* **Action:** Enabled dynamic prioritization of critical data paths (e.g., DMA vs control traffic), improving system robustness under high-concurrency workloads.
* **Result:** Successfully identified and resolved the bottleneck during post-silicon validation, with the fix integrated into the final production silicon.
* **Impact:** Introduced a **flexible arbitration** framework that improved system stability and provided firmware-controlled performance tuning for complex SoC workloads.
* **Takeaway:** Static arbitration is often insufficient for complex SoCs; implementing programmable priority registers is essential for robust, "deadlock-proof" multi-master designs.
</details>
