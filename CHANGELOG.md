## [2.1.1] - 2025-09-09

### Release Summary
Bug Fix Release

### Bugfixes
- TC-2733 Components missing from analysis/latest/component
- TC-2758 Listing latest components by CPE doesn't show all descendants defined in SBOMs
- TC-2701 Stage Atlas timeout for CPE cpe:/a:redhat:openstack:13::el7 with params descendants=10&limit=20&offset=0
- TC-2717 500 error when searching for purl using /analysis/latest/component/<value> endpoint

## [2.1.0] - 2025-07-28

### Release Summary
Bug Fix Release

### Minor Changes
- TC-2498 Use extensible labels to manage extensible metadata for SBOMs and Advisories

### Security Fixes

### Bugfixes
- TC-2606 Analysis/latest/component/<cpe> only returning a single root
- TC-2677 SBOM link regression on 0.3.z branch
- TC-2415 After uploading SBOM files with hundreds of CVEs, the dashboard page takes a lot of time to load and eventually shows an error
- TC-2562 Importer pod stuck in pending state for PVC
- TC-2418 Aggregate severity in a downloaded Advisory doesn't match the value displayed in the Advisory Explorer
- TC-2431 The number of the total advisories in the dashboard is not the same as in the advisories tab
- TC-2440 Search gets broken by tilde '~' character
- TC-2658 Vulnerabilities not reported for go package
- TC-2666 Labels - Field validation

## [2.0.1] - 2025-05-19

### Release Summary
Bug Fix Release

### Minor Changes
-TC-2488 Support custom trust anchors for S3

### Bugfixes
- TC-2441 Deleting a document leads to a stale broken data model
- TC-2469 Python package wrongly affected by vulnerability
- TC-2306 RHTPA 2.0: Support for minio endpoint
- TC-2473 TPA SBOM ingestion - performance issues
- TC-2489 CVSS scores with Environment or Temporal score component cause panic
- TC-2519 Vulnerabilities cannot be deleted due to foreign key constraints

## [2.0.0] - 2025-04-14

### Release Summary
First release based on trustify repository

### Minor Changes

### Security Fixes

### Bugfixes
