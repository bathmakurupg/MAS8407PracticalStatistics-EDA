# new-build


## Overview

This repository contains the centralized Jenkins pipeline used to build and publish  Deployable Units (DU) to Artifactory.

This is **Job 1** in the DU-based CI/CD model.

The purpose of this job is to:

* Pull new scoped application source code from GitHub
* Package it into a versioned Deployable Unit (DU)
* Generate checksum metadata
* Publish the DU artifact to JFrog Artifactory

This repository does not contain application source code.
It only contains CI/CD automation logic.

---

## Scope of This Repository

This repository is responsible for:

* Centralized DU packaging logic
* Versioned artifact generation
* Immutable storage in Artifactory
* Standardized build process across new applications

It does **not** handle:

* Deployment to QA/UAT/Production
* Environment promotion
* ATF execution


## Credentials & Access

This pipeline requires:

* GitHub read access
* Artifactory deploy access (Generic Local repository)
* Jenkins job-level credentials configuration

No credentials are stored in this repository.

---

## Current Status

This repository is part of a Proof of Concept (PoC) for implementing a DU-based CI/CD model for new Smart Applications.


