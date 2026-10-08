# Cynapsa Core wheels

This repository holds downloadable, platform-specific Python wheels containing
the Cynapsa Go Core shared library. Wheels are built from the
[`cynapsagocore`](https://github.com/Cynapsa/cynapsagocore) release workflow;
the exact source commit and native-library SHA-256 are recorded inside each
wheel's `cynapsa_core/_build.json`.

When a release is available, download the wheel matching your OS and CPU from
[Releases](https://github.com/Cynapsa/cynapsa-core-wheels/releases), verify it
against the attached `SHA256SUMS`, then install that file with `pip install`.
These are native-library wheels, not the Python SDK. The SDK does not yet
automatically discover a separately installed Core wheel; point
`CYNAPSA_CORE_LIBRARY` at the installed shared library when using them together.

Initial releases are marked **pre-release** while platform qualification is
ongoing. The absence of a wheel for a platform or a particular release does
not imply production support.
