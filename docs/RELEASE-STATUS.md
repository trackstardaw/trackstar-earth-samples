# Release status

`earth-v1-staging` is intentionally pending ingest. The manifest has 17 instruments and each note path is reserved for a future release asset. Do not mark an instrument `ready` until all of its promised note assets have been uploaded and verified.

Required checks before production wiring:

- release manifest is reachable over HTTPS;
- each uploaded WAV returns 200;
- representative WAV requests support `Range: bytes=0-1023` with 206;
- browser CORS and fetch succeed from the EdgeOne origin;
- a human listens to the QA C-major scales and confirms they sound like the named instruments.
