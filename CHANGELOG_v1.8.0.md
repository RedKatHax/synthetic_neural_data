# Ok-aSTEM Repository Changelog — v1.8.0

**Release Date:** 2025-10-18  
**Maintainers:** Kim + K.A.I.R.A.  

## Summary
Adds labeled perturbation epochs and a QC pipeline to validate coupling shifts across epochs. Builds on v1.7.0 (panel with inhibitory pulses) by introducing an excitatory epoch and per-epoch analytics.

### 🔄 Changes
- New dataset: `synthetic_neural_data_v1.8.0_panel_labeled_epochs.csv`
  - Labeled epochs: pre_baseline (0–499 ms), inhibitory_500_700 (500–700 ms), mid_baseline (701–1199 ms), excitatory_1200_1300 (1200–1300 ms), post_baseline (1301+ ms)
  - Retains inhibitory pulses and adds excitatory burst adjustments
- QC assets:
  - `qc_epoch_correlations_v1.8.0.csv` (Pearson r(Vm, FR) per neuron per epoch)
  - `QC_Report_v1.8.0.ipynb` (recomputes summary pivots, plots distributions, and visualizes traces)
- Provenance manifests retained from v1.7.0:
  - `neuron_param_manifest_v1.7.0.csv` and `.json` (per-neuron parameter priors and perturbation strengths)
