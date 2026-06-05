# Wei_project
Overview of the project

This project investigates the neurophysiological boundaries of human mental workload and cognitive resilience. By combining behavioral tracking with high-temporal-resolution electroencephalography (EEG), the study maps how individuals with High Working Memory Capacity (HWM) and Low Working Memory Capacity (LWM) differ when navigating extreme mental stress and recovering from cognitive failures. The project leverages event-related potentials (ERPs)—specifically the P300 wave recorded at the parietal site (Pz)—to provide direct, objective evidence of executive brain function in real time.

Core Objectives & Hypotheses

Phase 1: The Capacity Limits & Cognitive Load Hypothesis

Objective: Map the trajectory of attention deployment as task difficulty increases.

Hypothesis: Brain resource mobilization does not drop uniformly for everyone. Instead, as task demands grow linearly from 1-back to 4-back, HWM individuals will demonstrate optimal, flexible resource allocation, dropping peak activity early when a load becomes inefficient. LWM individuals will exhibit a delayed, rigid "over-mobilization" strategy before hitting a cognitive ceiling.

Phase 2: Post-Error Adaptation Hypothesis

Objective: Capture how the central executive network dynamically reacts immediately following a psychological mistake.

Hypothesis: When looking at Trial n+1 immediately following an error on Trial n, HWM individuals will show a highly adaptive, binary neural response—displaying a dramatic P300 "Rebound Effect" during successful recovery, and a sharp neural collapse when choosing to disengage (giving up). Conversely, LWM individuals will show "Neural Rigidity," where their brain waves fail to adjust dynamically regardless of whether they randomly pass or fail the next trial.

3. Experimental Methodology & Technology

Task Paradigm: A continuous visual N-back task spanning four distinct difficulty blocks (1-back, 2-back, 3-back, and 4-back).
Data Volume: 18 continuous BrainVision EEG datasets parsed into two strictly balanced operational cohorts (HWM vs. LWM).
Technical Pipeline: * Advanced BIDS alignment merging continuous signal files (.vhdr) with independent external behavioral logs (_events.tsv) to bypass missing hardware markers.
Digital bandpass filtering (0.1 Hz to 30.0 Hz) to isolate true cortical oscillations while neutralizing muscle artifacts and slow drift.
Stimulus-locked and performance-locked Epoching (-200 ms to 800 ms) with exact pre-stimulus baseline correction.Microvolt time-series quantification isolated to the Pz electrode channel within the standard 300–550 ms P300 window.
