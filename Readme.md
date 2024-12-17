# BioHackRxiv for the SpatialData Developer Workshop
Basel, 2024
Pre-print published here: https://osf.io/preprints/osf/u2a6m?view_only=.

## How to Build

Instructions and examples are available [here](https://github.com/biohackrxiv/bhxiv-gen-pdf/).

1. **Build the required Docker container** (this process takes 5-10 minutes):
   ```bash
   docker build -t biohackrxiv/gen-pdf:local -f docker/Dockerfile .
   ```

2. **Build the .pdf**:
   ```bash
   docker run --rm -it -v $(pwd):/work -w /work biohackrxiv/gen-pdf:local gen-pdf .
   ```
