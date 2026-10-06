## [3.1.1] - 2026-10-13

### Release Summary
Bug fix and improvement release
Third deprecated version

### Bugfixes
- TC-4926 UI - Intermittent Read-only warning message
- TC-5690 Improve the efficiency of the 3.0 Migration scripts for Advisories
- TC-5722 Operator's excludes.json incorrectly excludes node_modules for JavaScript, breaking reachability analysis
- TC-5738 Unified importer credential resolution with external secret store support
- TC-5764 HTTP transport with Pulp Manifest file discovery
- TC-5996 Replace hardcoded recommendation regex with configurable env var
- TC-5997 Add recommendation DB entity and migration
- TC-5998 OSV advisory ingestor hook and reindex endpoint
- TC-5999 Recommendation report endpoint (POST /v3/recommend/report)
- TC-6000 Extend SBOM queries with recommendation JOIN and aggregate count
- TC-6001 Recommendation column in SBOM packages view and packages list page
- TC-6002 Recommendation column in SBOM vulnerabilities view
- TC-6003 Aggregate remediation count on SBOMs list page
- TC-6004 Remediation report page and SBOMs list report button
- TC-6061 Accept CycloneDX 1.7 SBOMs at ingestion (version gate + fixture + tests)
- TC-6068 Ingest CycloneDX extended license details into licensing_infos
- TC-6090 Define shared auth model, update Quay importer, and add data migration
- TC-6091 Update NVD, KEV, and ClearlyDefined runners to use shared HTTP client builder
- TC-6229 HTTP transport core: pluggable discovery trait + shared retrieval/integrity layer
- TC-6230 Pulp Manifest discovery strategy for the HTTP transport
- TC-6231 Http importer config + run_once_http runner + auth + schema/OpenAPI regen
- TC-6251 Return 503 FEATURE_UNCONFIGURED when /recommend called without TRUSTD_RECOMMEND_PATTERNS set
- TC-6303 Expose fixed_versions in PurlStatus and has_fix_versions filter (v2 and v3)
- TC-6305 Strengthen fetch-failure test: assert Retrieval phase, URL, and error message
- TC-6319 Fix fixed_versions to serialize as [] when empty (remove skip_serializing_if)
- TC-6398 Recommendation column in global Packages page, Vulnerabilities page, and Package detail Vulnerabilities tab
- TC-6411 Fix: fetch_retries silently ignored for authenticated HTTP imports (TC-6231)
- TC-6412 Fix: Bearer/API-key credentials from files fail with trailing newline
- TC-6413 Fix: inline qualified paths in build_fetcher violate CONVENTIONS.md import style

## [3.1.0] - 2026-08-13

### Release Summary
EI integration
Second deprecated version

### Bugfixes

## [3.0.0] - 2026-07-23

### Release Summary
First deprecated version

### Bugfixes
- TC-2402 UX quirks related to filtering by date
- TC-2422 Changing the "From" field of the calendar deletes the "To" field completely
- TC-2520 CSAF Advisories with a CVSS vector containing an Environment or Temporal score fail to upload
- TC-3051 UI: SBOM Details - Packages Tab - Long licenses occupy too much space
- TC-3143 Vulnerability score accidentaly picked from CVE instead of GHSA
- TC-3212 Slow performance of analysis endpoints
- TC-3248 Upload advisory button on Search page
- TC-3265 "client_id is not present" when logout
- TC-3268 Selection of a single SBOM on the Dashboard page causes all 4 SBOMs to reload
- TC-3294 Opening link for Packager or SBOMs related to Licenses in new window ignores the filter
- TC-3370 RHTPA - UI - Page title does not change based on viewed page
- TC-3742 Slow TPA responses
- TC-4734 CVSSv4 ProviderUrgency (U) metric fails to parse valid values
- TC-5163 Git-based importers (CVE, OSV) ignore proxy configuration due to missing ProxyOptions in libgit2 FetchOptions

## [2.2.6] - 2026-07-22

### Release Summary
Bug fix Release
### Bugfixes
- TC-5163 Git-based importers (CVE, OSV) ignore proxy configuration

## [2.2.5] - 2026-06-25

### Release Summary
Bug fix Release
### Bugfixes
- TC-4542 Improve behaviour of cache then it's under memory pressure
### Minor Changes
- TC-4162 Create a read only/kill switch for TPA

## [2.2.4] - 2026-04-20

### Release Summary
Bug fix Release
### Bugfixes
- TC-3623 OIDC userinfo call fails for Azure Entra as OIDC
- TC-4108 Add OIDC_LOAD_USER configuration support to server API

## [2.2.3] - 2026-03-31

### Release Summary
Bug fix Release
### Bugfixes
- TC-3742 Slow TPA responses
- TC-3745 RHTPA UI - re-executes endpoint that fails
- TC-3762 UIScopes field for OIDC

### Minor Changes
- TC-3751	Identify Red Hat SBOMs using case insensitive Organization

## [2.2.2] - 2026-02-25

### Release Summary
Bug fix Release
### Bugfixes
- TC-3624 Can't find some components in latest analysis endpoint

## [2.2.1] - 2026-02-19

### Release Summary
Bug fix Release

### Bugfixes
- TC-2717 500 error when searching for purl using /analysis/latest/component/<value> endpoint
- TC-2848 After an SBOM is deleted, there are errors displayed in the Dashboar
- TC-2985 Scan SBOM Report Failed screen UX mistmatch cod Client side validation
- TC-3037 CBOM: Cannot read properties of undefined (reading uui) erorr on SBOM details page
- TC-3073 Missing result in latest returned by non-latest endpoint
- TC-3170 Query latest (and non latest) endpoints omits "anchestors"
- TC-3201 Github CVE Importer error - data did not match any variant of untagged enum
- TC-3212 Slow performance of analysis endpoints
- TC-3214 Improve source_document deletes
- TC-3234 Concurrent upload: refactoring
- TC-3278 Latest endpoint only returning one result where non-latest returns many
- TC-3286 q processing mismatch for in-memory vs DB for PURLS of SBOMs
- TC 3432 Metrics not matching the right path for /reccomend and /analyze

## [2.2.0] - 2025-11-25

### Release Summary
Bug fix and enhance release

### Bugfixes
- TC-2414 Version 2 - License Export SPDX package CPE mismatches to SBOM
- TC-2598 Vulnerabilities table - Inconsistent CVSS column sorting
- TC-2615 Performance issues with DELETE /api/v2/sbom/{id} endpoint
- TC-2675 No error is reported in the UI when pointing the Quay importer to a non-existent source
- TC-2685 When disabling a running Quay importer, the message diplayed in the UI is wrong
- TC-2686 When an image tag expires in the repository before the importer digests it, there is a nasty error message in the UI under the importer
- TC-2805 SBOM with vulnerable packages shows 0 vulnerabilities
- TC-2980 Scan SBOM - Report generated only with Affected vulnerabilities - Remove Status filter
- TC-2983 OSV Vulnerability not reported on TPA
- TC-3003 Remove PURL GC endpoint
- TC-3007 Scan SBOM - Static Spinner while uploading sbom and Generating reports
- TC-3152 Concurrent upload: duplicate key value violates unique constraint error
- TC-3176 SBOM and Vulnerability deadlocks fix
- TC-3177 zstd encoding is broken

### Minor Changes
- TC-2824 AIBOM/CBOM Ingestion and retrieval Task
- TC-2828 Create an ADR for extracting recommendations information from OSV and CSAF
- TC-2948 Implementation of the recommendation API endpoint
- TC-2981 License filtering: consistently update current SBOM packages license filter

## [2.1.1] - 2025-09-15

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
- TC-2488 Support custom trust anchors for S3

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
