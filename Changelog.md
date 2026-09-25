# Changes to Windows-2025-CIS-Audit

## Based on CIS Benchmark v1.0.0
## September 2026 - stand-alone servers

- spec folders for sections 1, 5, 9 and 19 split by subsection, .x suffix dropped
- 18 MS only controls asserted on any server that is not a domain controller
- 2.3.6.x asserted on domain controllers
- 2.2.31 asserts LOCAL SERVICE, NETWORK SERVICE and RESTRICTED SERVICES\PrintSpoolerService, matching the role
- README: stand-alone server scope
- README: NGWS switch, 2.2.31 asserts the v2.1.0 value

## September 2026 - NIST and domain members

- NIST800-53R5 added to meta, taken from the role's NIST tags
  - The benchmark JSON carries GRID references only
  - 19.5.1.1 has no NIST tag, so no field
- 2.3.11.6 asserted on standalone hosts only
- Section 1 account policy and 2.3.11.6 reported as skipped on a domain joined host, with the reason in meta.skip_reason
- README covers 2.3.11.6 on domain members
- Spec folders follow the role's new task files
  - section01, section05, section09, section19 replaced by section_1.1.x, section_1.2.x, section_5.x, section_9.x, section_19.x

## 1.0.0 based on CIS Benchmark v1.0.0

- Initial release - beta, pending feedback. Please raise an issue or reach us on
  Discord with anything it gets wrong, reports unexpectedly, or misses
