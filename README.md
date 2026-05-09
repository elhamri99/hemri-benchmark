# HEMRI — Neural Spike Sorting Pipeline

Cloud pipeline for automated spike sorting of extracellular 
electrophysiology recordings.

**Upload raw recording → get sorted neurons + quality metrics back.
No HPC. No setup. One API call.**

---

## Benchmark Results

Tested using SpikeInterface framework with tridesclous2 sorter.
Preprocessing: bandpass filter (300-6000 Hz) + common median reference.

| Configuration       | Accuracy | Precision | Recall | ISI Violation |
|---------------------|----------|-----------|--------|---------------|
| Small probe 16ch    | 98.9%    | 99.9%     | 98.9%  | 0.00%         |
| Dense probe 100ch   | 85.1%    | 86.0%     | 85.1%  | 0.02%         |
| Harris 2000 baseline| 70.0%    | —         | —      | —             |

hemri_benchmark_final.png

---

## Pipeline
