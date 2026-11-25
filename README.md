# EEGLAB to mne/raw

<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

**Converts EEG data in EEGLAB format (.set/.fdt) to an MNE-Python Raw .fif file; a format conversion utility.**

Reads the EEGLAB .set file with mne.io.read_raw_eeglab and saves it as raw.fif. BIDS sidecar files (channels, electrodes, coordsystem, events) are accepted with the input but not copied or applied by the current code.

Run it on brainlife.io: [https://doi.org/10.25663/brainlife.app.633](https://doi.org/10.25663/brainlife.app.633)

| Input | Datatype | Required | Description |
|---|---|---|---|
| `eeglab1` | `neuro/eeg/eeglab` | yes | EEG recording in EEGLAB format (.set with .fdt) and BIDS sidecars. |

| Output | Datatype | Description |
|---|---|---|
| `out_dir` | `neuro/meeg/mne/raw` | MNE Raw data in FIF format |

Runtime: container `brainlife/mne:0.23dev`; 8 CPUs.

<!-- brainlife-app:end -->

