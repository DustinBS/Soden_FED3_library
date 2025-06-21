See the original repo for more context. This fork has the following changelist:
#### Unlimited Pellet Retrieval Time
* Removed the 60-second pellet retrieval limit; retrieval time is now unlimited.
* 1ms temporal resolution timer for the first 5 minutes, then switches to low-power (~500ms temporal resolution) for extended retrievals.
* In retrieval time display, shows `ms` for < 100 seconds, and `X.Xs` for longer durations (e.g., `115.2s`).

#### Expanded Device ID Support

* 4-digit device IDs (1-9999) across device settings, on-screen display, and data filenames (e.g., `FEDXXXX_MMDDYY_NN.CSV`).

#### Automatic Session Start Logging

* Logs an `EstimatedStart` event at session initiation to capture device start timestamp. I use this for syncing experiments.
