# Changes to Windows-2025-CIS-Audit

## Based on CIS Benchmark v2.1.0

- spec folders for sections 1, 5, 9 and 19 split by subsection, .x suffix dropped
- 96 manifest entries for missing spec files removed
- 17 MS only controls and 5.2 Print Spooler asserted on standalone servers
- 2.3.6.x asserted on domain controllers
- README: stand-alone server scope and the NGWS switch
- Benchmark version v1.0.0 to v2.1.0
- Specs regenerated from the upgraded remediation role
- 126 controls renumbered
- 43 controls retired, including the 18.10.43 Defender Antivirus group
- 9 controls added: 18.7.14-18.7.18, 18.9.7.2, 18.9.17.1, 18.11.1, 18.11.2
- Renumbered specs moved to their new section folders
- 17.8.1 asserts Success only
- 2.2.30, 2.2.31, 2.2.32 include RESTRICTED SERVICES\PrintSpoolerService
- 2.2.30 asserts LOCAL SERVICE, NETWORK SERVICE instead of NONE
- 18.9.27.1 asserted on domain controllers only
- 18.9.41.3 asserts ROCA validation Block
- 2.3.5.4 asserts LDAPServerEnforceIntegrity
- 18.9.19.5 asserts DisableBkGndGroupPolicy is absent
- 18.9.27.2 asserts RunAsPPL in the Windows System policy key
- run_audit.ps1 BenchmarkVer 2.1.0
- README profile counts and control references updated
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
