## Low-latency Pitch-Shifting with STN decomposition
Semester Project for SMC9 AAU CPH. Accepted for publication in Conference Proceedings DAS | DAGA 2025. 

### Description

This repository hosts the code and resources for implementing a novel real-time pitch-shifting algorithm designed for complex audio signals. The project integrates fuzzy Sines-Transient-Noise (STN) decomposition with specialized processing pipelines for sines, transient, and noise components.

Developed as a VST audio plug-in using the JUCE framework, the system allows precise pitch adjustments across a wide range of semitones. It is optimized for real-time performance and features user-configurable parameters, such as pitch-shift range, decomposition bounds, and FFT size.

### Key Features

- Sines-Transient-Noise (STN) Decomposition: Separates audio into distinct components for targeted processing
- Specialized Algorithms: Noise Morphing and "Vase-Phocoder" for enhanced pitch-shifting quality
- Real-Time Processing: Low-latency implementation for live applications
- User-friendly interface with adjustable parameters for precise sound design

#### Online modifications 
<!-- TODO Add graphics  -->

### Evaluation

The system has been tested through blind listening experiments and interviews, comparing its performance to commercial alternatives. While the current version shows artistic potential, ongoing work focuses on improving audio quality, optimizing computational performance, and refining evaluation methodologies.

#### Wilcoxon signed-rank and Cliff's $\delta$ analysis
<!-- % TODO Table to be found on github repo and website
% \begin{table*}[t]
%     \centering
%     \caption{Wilcoxon signed-rank and Cliff's $\delta$ analysis}
%     \vspace{2mm}
%     \label{tab:wilcoxon}
%         \begin{tabularx}{14cm}{@{\arrayrulewidth1.5pt\vline}B|B|B|B|B@{\arrayrulewidth1.5pt\vline}}
%             \noalign{\hrule height1.5pt} 
%             Pairing & p-value           & Cliff's $\delta$  & Magnitude & CI                \\
%             \noalign{\hrule height1.5pt}
%             AN - PS & \num{5.17e-09}    & 0.852             & Large     & $(0.673, 0.937)$  \\ \hline 
%             PS - EL & \num{5.54e-07}    & 0.581             & Large     & $(0.359, 0.741)$  \\ \hline 
%             PS - WS & \num{3.18e-12}    & 0.743             & Large     & $(0.563, 0.856)$  \\ \hline 
%             PS - SS & $0.0004$          & 0.433             & Medium    & $(0.208, 0.615)$  \\
%             \noalign{\hrule height1.5pt}
%         \end{tabularx}
% \end{table*} -->


### Future Plans

- Audio quality enhancements
- Performance optimization
- Improved evaluation strategies

### Set-Up Notes

This project includes 3 external dependecies setup as submodules: webMUSRHA and signalsmith DSP libraries.
