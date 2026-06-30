[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.on008062-blue)](https://doi.org/10.82901/nemar.on008062)

EEG and liking responses to sonic-seasoning soundscapes.

Per participant: one combined EEG file (eyes-open + eyes-closed baseline + ~17 s exposure to jungle and deconstruct
soundscapes), events.tsv marking segments, with liking ratings and baseline-state survey items in participants.tsv,
and stimulus audio in /stimuli. Released as recorded (EPOC X hardware bandpass only; no additional software filtering). Recording timestamps removed.
Participant IDs are de-identified (sequential sub-NN); the mapping to original recording IDs is held privately and
is not part of this dataset. See the associated Data in Brief article for full description.

EEGLAB USERS
------------
A processed, EEGLAB-ready version of the two soundscape conditions (jungle, deconstruct)
is provided under derivatives/eeglab/ as per-condition .set files that import directly
into an EEGLAB STUDY with conditions assigned. See derivatives/eeglab/README for details.
The raw combined EDFs at the repository root remain the primary, archival data.

RESTING CALIBRATION (eyes-open / eyes-closed) — IMPORTANT NOTE
-------------------------------------------------------------
The eyes-open and eyes-closed calibration segments had a fixed intended duration of
~20 s each, but in the experiment builder each advanced on a participant-controlled
"continue" button (not a hard timer). Segment markers therefore span from segment
start to that button press, so recorded durations vary across participants
(eyes-open mostly ~24 s, a few longer; eyes-closed ~26-63 s), and the button-press
times were not logged. The full segments are released unmodified.
=> For length-matched comparisons (e.g. with the 17 s soundscape exposures), use the
   FIRST 17 s of each calibration segment: it falls within the fixed instructed window
   for all participants and precedes any post-task advance interval.
