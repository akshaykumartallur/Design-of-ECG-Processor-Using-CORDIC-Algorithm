<h1>Design of ECG processor using CORDIC Algorithm</h1>

  <h2>Overview</h2>
  <p>
    This project implements a resource-efficient ECG signal processor using the CORDIC (COordinate Rotation DIgital Computer) algorithm.
    Designed in SystemVerilog and simulated using Vivado, it enables real-time R-peak detection and average heart rate calculation
    without requiring power-hungry multipliers, making it ideal for wearable biomedical devices.
  </p>

  <h2>Key Features</h2>
  <ul>
    <li>CORDIC-based magnitude calculation with zero DSP multiplier usage</li>
    <li>QRS peak detection using adaptive threshold logic</li>
    <li>RR interval and BPM estimation with real-time tracking</li>
    <li>Arrhythmia detection support based on average heart rate analysis</li>
    <li>Tested with MIT-BIH Arrhythmia Database ECG signals</li>
  </ul>


  <h2>How It Works</h2>
  <p>
    The ECG input (in .txt format) is fed into a SystemVerilog testbench. The design detects R-peaks, calculates RR intervals, and
    outputs BPM values. Based on the computed average BPM, the processor identifies the cardiac condition as Normal, Bradycardia,
    or Tachycardia. Results are printed to the simulation console.
  </p>

  <h2>Simulation Output</h2>
  <ul>
    <li>RR intervals (in milliseconds)</li>
    <li>Beat-to-beat BPM</li>
    <li>Final average BPM</li>
    <li>Conclusion: Normal, Bradycardia, or Tachycardia</li>
  </ul>

  <h2>Tools Used</h2>
  <ul>
    <li><strong>Vivado 2024.2</strong> – Design simulation and analysis</li>
    <li><strong>SystemVerilog</strong> – RTL modeling</li>
    <li><strong>MATLAB / Python</strong> – ECG data processing (optional)</li>
    <li><strong>MIT-BIH Database</strong> – Testing dataset</li>
  </ul>

  <h2>Status</h2>
  <p>Phase-I Completed: RTL modules verified with MIT-BIH records. Report finalized. Phase-II will focus on hardware synthesis and real-time interfacing.</p>

  <h2>Contributors</h2>
  <ul>
    <li>Abhay Surya Shankar – 1DS22EC004</li>
    <li>Akshaykumar Tallur – 1DS22EC023</li>
    <li>Bhavya Y – 1DS22EC048</li>
    <li>Deepthi S R – 1DS22EC059</li>
  </ul>



  <h1>Project Diary</h1>
  <p><strong>Project Title:</strong>Design of ECG Processor Using CORDIC Algorithm</p>
  <p><strong>Guide:</strong> Dr. Vimala P</p>
  <p><strong>Team Members:</strong> Abhay Surya Shankar, Akshaykumar Tallur, Bhavya Y, Deepthi S R</p>


  <hr>

  <h2>23 August 2025</h2>
  <p><strong>Work Summary:</strong> We officially kicked off the project by selecting our topic: building an ECG processor using the CORDIC algorithm. Our team met regularly to divide initial responsibilities, explore previous ECG-related work, and gather relevant papers. We also became familiar with the MIT-BIH database and set up our development environment using Vivado.</p>
  <p><strong>Hours Worked:</strong> 7 hours</p>
  <p><strong>Learnings:</strong>We learned the significance of QRS complexes in ECGs and how digital signal processing plays a key role in heart rhythm analysis. We also got our first exposure to the CORDIC method and how it's used to simplify mathematical computations.</p>
  <p><strong>Blockers/Risks:</strong>Understanding the raw ECG data format from MIT-BIH took some time. We also spent effort figuring out a clean project structure and data visualization tools.</p>


  <h2>20 September 2025</h2>
  <p><strong>Work Summary:</strong>we modeled basic signal processing blocks using verilog. We focused on implementing the CORDIC-based magnitude computation unit in vectoring mode. We also developed a five-point derivative module to emphasize slope changes and started creating a testbench with real ECG samples.</p>
  <p><strong>Hours Worked:</strong> 13 hours</p>
  <p><strong>Learnings:</strong>We understood how bit-shifting and iterative vector rotations could replace complex multipliers. Working on the derivative operator helped us detect slope shifts related to the QRS complex.</p>
  <p><strong>Blockers/Risks:</strong>Verifying the CORDIC block for accurate magnitude under various edge cases needed time. Also, setting correct data widths to avoid overflow or underflow was a learning curve.</p>
 

  <h2>15 October 2025</h2>
  <p><strong>Work Summary:</strong>We integrated the CORDIC and derivative modules and added a moving window integrator to smooth out outputs. A custom peak detection logic with adaptive thresholding was created. We also started verifying R-peak timing from MIT-BIH input.</p>
  <p><strong>Hours Worked:</strong> 7 hours</p>
  <p><strong>Learnings:</strong>We explored threshold tuning to adapt dynamically to real ECG signals. Building state machines for peak detection gave us better control over how beats are identified accurately without needing filters.</p>
  <p><strong>Blockers/Risks:</strong>Some false positives occurred when peaks were too close. Tuning the refractory period and window size helped improve detection.</p>


  <h2>14 November 2025</h2>
  <p><strong>Work Summary:</strong>We introduced RR interval measurement and converted it into BPM calculation. The classification module was added to detect rhythm categories such as normal, bradycardia, and tachycardia. We validated BPM output using multiple patient records.</p>
  <p><strong>Hours Worked:</strong> 13 hours</p>
  <p><strong>Learnings:</strong>RR intervals proved to be an elegant way to estimate heart rate without relying on continuous filtering. We learned how to label and map BPM values to probable heart conditions.</p>
  <p><strong>Blockers/Risks:</strong>We had to debug timing alignment between peaks and BPM calculation. Handling missing or irregular peaks required careful exception logic.</p>


  <h2>5 December 2025</h2>
  <p><strong>Work Summary:</strong>We expanded the testbench for bulk testing across datasets like record 100 and 200. A final output block was added to display summary results: average BPM and detected condition (e.g., normal or bradycardia). Output was cleaned for readability.</p>
  <p><strong>Hours Worked:</strong> 8 hours</p>
  <p><strong>Learnings:</strong>Summarizing results at the end of the simulation gave us a clear understanding of performance over long data windows. We also learned how to trace BPM trends across time.</p>
  <p><strong>Blockers/Risks:</strong>Managing long simulations with large files tested our patience and system stability. Keeping waveform display aligned with final outputs was another challenge.</p>

