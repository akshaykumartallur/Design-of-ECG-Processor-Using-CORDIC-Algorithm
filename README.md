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


</body>
</html>
