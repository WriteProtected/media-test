# WriteProtected media test

Public, synthetic-only acceptance fixtures for the WriteProtected BackOffice JPEG
upload workflow. This repository is separate from `WriteProtected/media` and is
not connected to the public catalogue or any website deployment.

Upload branches are public before merge. Do not upload personal photographs,
private catalogue data, credentials or camera metadata from real users here.

Tests use an isolated BackOffice application, disposable catalogue/private schemas
and separate file, mirror and credential directories. Tokens must be fine-grained,
limited to this repository with Contents read/write, and short-lived.

Photo branches use `photos/bo-<batch-id>`. Their merge is an explicit owner test step.
The application never merges branches or publishes a website automatically.
