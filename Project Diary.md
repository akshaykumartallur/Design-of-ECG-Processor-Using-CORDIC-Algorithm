  <h1>Project Diary</h1>
  <p><strong>Project Title:</strong>Design of ECG Processor Using CORDIC Algorithm</p>
  <p><strong>Team Members:</strong> Abhay Surya Shankar, Akshaykumar Tallur, Bhavya Y, Deepthi S R</p>
  <p><strong>Guide:</strong> Dr. Vimala P</p>


  <hr>

  <h2>August 2025</h2>
  <p><strong>Work Summary:</strong> We began the project by finalizing our topic after evaluating several options under the bio-medical signal processing domain. Once we chose the CORDIC-based ECG processor, we researched its relevance and feasibility. Team responsibilities were distributed, and a preliminary timeline was created.</p>
  <p><strong>Hours Worked:</strong> ~15 hours</p>
  <p><strong>Learnings:</strong> Basics of ECG waveform (PQRST) and its diagnostic significance, Introduction to CORDIC algorithm and its role in low-power computing</p>
  <p><strong>Blockers/Risks:</strong> Lack of familiarity with ECG data handling, Uncertainty around simulation complexity</p>
  <p><strong>Skills Acquired:</strong> Literature review, Team coordination, Time-bound planning</p>

  <h2>September 2025</h2>
  <p><strong>Work Summary:</strong> This month was focused on deep literature exploration. We studied the Pan-Tompkins algorithm, existing FPGA-based ECG processors, and reviewed MIT-BIH Arrhythmia data formats. We also began understanding SystemVerilog for digital design.</p>
  <p><strong>Hours Worked:</strong> ~22 hours</p>
  <p><strong>Learnings:</strong> FPGA architecture basics, MIT-BIH database annotation formats, Difference between DSP and CORDIC computation techniques</p>
  <p><strong>Blockers/Risks:</strong> Interpreting annotated ECG files, Complexity of QRS detection logic</p>
  <p><strong>Skills Acquired:</strong> Technical documentation extraction, HDL design fundamentals, Collaborative research</p>

  <h2>October 2025</h2>
  <p><strong>Work Summary:</strong> We initiated module-level design for the ECG signal processor. A pipeline was planned with core stages: data input, R-peak detection, RR interval calculation, and BPM classification. CORDIC implementation was prototyped.</p>
  <p><strong>Hours Worked:</strong> ~28 hours</p>
  <p><strong>Learnings:</strong> Shift-add operations in CORDIC, RTL structure and pipeline planning, FIFO buffer modeling for sample streaming</p>
  <p><strong>Blockers/Risks:</strong> Simulation misbehavior due to time delays, No standard testbench pattern initially</p>
  <p><strong>Skills Acquired:</strong> Modular RTL coding, Simulation with test vectors, Debugging procedural logic</p>

  <h2>November 2025</h2>
  <p><strong>Work Summary:</strong> Core SystemVerilog design files were finalized and integrated. Testbenches were written for unit testing. We processed sample ECG records and generated output BPM values for verification. Early performance data was recorded.</p>
  <p><strong>Hours Worked:</strong> ~30 hours</p>
  <p><strong>Learnings:</strong> Testbench creation and waveform tracing, BPM computation logic and corner-case handling, Role of thresholds in peak detection</p>
  <p><strong>Blockers/Risks:</strong> Inconsistent simulation outputs with noisy data, Difficulty in handling large sample inputs</p>
  <p><strong>Skills Acquired:</strong> Functional simulation in Vivado, Handling real-world datasets, Analytical result interpretation</p>

  <h2>December 2025</h2>
  <p><strong>Work Summary:</strong> A robust simulation environment was built using actual MIT-BIH samples. We analyzed performance for both normal and diseased records. The conclusion logic (Normal/Bradycardia/Tachycardia) was added to the testbench.</p>
  <p><strong>Hours Worked:</strong> ~25 hours</p>
  <p><strong>Learnings:</strong> Heart rate thresholds and clinical norms, Variability in diseased records, Timing synchronization in testbench</p>
  <p><strong>Blockers/Risks:</strong> Slow simulation for large datasets, Potential accuracy drop for edge cases</p>
  <p><strong>Skills Acquired:</strong> Data-driven testing, Diagnostic classification logic, Simulation automation</p>
