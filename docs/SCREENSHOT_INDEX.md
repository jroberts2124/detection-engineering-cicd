# Detection Engineering Screenshot Index

All 29 screenshots extracted from `new soc.docx` are included and renamed in chronological order.

## Recommended README screenshots

Use these as the main evidence in the GitHub README:

1. `01-splunk-forwarder-and-test-event.png` - Confirms the Splunk Universal Forwarder is running and telemetry reaches the pipeline.
2. `05-atomic-red-team-fileless-execution-success.png` - Shows successful execution of the controlled T1059.001 test.
3. `07-powershell-4104-script-block-evidence.png` - Shows suspicious PowerShell script-block telemetry in Splunk.
4. `08-sysmon-powershell-process-evidence.png` - Shows Sysmon process-creation evidence for PowerShell.
5. `11-brute-force-failed-logon-aggregation.png` - Shows five failed logons grouped into a brute-force signal.
6. `14-multi-source-correlation-result.png` - Strongest detection screenshot: five failed logons, successful logon, PowerShell process, suspicious script, and a 534.8-second chain.
7. `16-sigma-rule-validation.png` - Shows all Sigma rules passing validation.
8. `21-multi-source-sigma-conversion.png` - Shows the multi-source Sigma bundle converting to Splunk SPL.
9. `22-generalized-multi-source-detection-results.png` - Shows the reusable generalized detection producing correlated results.
10. `24-contentctl-validation-success.png` - Shows the contentctl project passing validation.
11. `27-contentctl-build-success.png` - Shows successful generation of the deployable Splunk content pack.
12. `28-packaged-splunk-detection.png` - Shows the detection inside the generated `savedsearches.conf` package.
13. `29-github-actions-success.png` - Shows the complete GitHub Actions validation/build pipeline passing.

## Supporting screenshots

- `02-powershell-4104-pipeline-test.png` - PowerShell 4104 ingestion test.
- `03-atomic-red-team-t1059-setup.png` - Atomic Red Team module and technique setup.
- `04-atomic-red-team-fileless-test-details.png` - T1059.001 fileless test definition and commands.
- `06-splunk-suspicious-powershell-search.png` - Suspicious PowerShell hunting query.
- `09-brute-force-simulation.png` - Controlled failed-authentication generation.
- `10-windows-4625-failed-logon-events.png` - Individual Windows 4625 events.
- `12-windows-4624-successful-logon-events.png` - Windows 4624 successful-logon events.
- `13-multi-source-correlation-spl.png` - Custom correlation SPL.
- `15-sigma-splunk-pipelines.png` - Installed Sigma processing pipelines.
- `17-sigma-to-splunk-conversion.png` - Basic Sigma-to-Splunk conversion.
- `18-sigma-sysmon-spl-search.png` - Converted Sysmon SPL search.
- `19-sigma-sysmon-spl-results.png` - Converted Sysmon search results.
- `20-sigma-bruteforce-spl-validation.png` - Converted brute-force SPL and results.
- `23-contentctl-detection-creation.png` - Interactive contentctl detection creation.
- `25-contentctl-build-output.png` - contentctl build progress.
- `26-content-pack-artifacts.png` - Generated content-pack file structure.

## Suggested README order

For a concise recruiter-facing story, embed screenshots in this order:

1. Telemetry collection: `01`
2. Attack simulation: `05`
3. PowerShell evidence: `07` and `08`
4. Authentication detection: `11`
5. Correlation result: `14`
6. Sigma validation/conversion: `16` and `21`
7. contentctl validation/package: `24`, `27`, and `28`
8. CI/CD proof: `29`

Keep the remaining images in `docs/screenshots` as supporting evidence and link to the directory instead of embedding every image in the README.
