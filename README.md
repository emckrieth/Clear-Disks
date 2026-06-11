# Clear Disks

A PowerShell disk sanitation utility that lists attached disks, prompts for an explicit disk selection, requires typed confirmation, and uses DiskPart to run destructive disk-cleaning operations.

## What It Demonstrates

- PowerShell scripting for Windows administration
- Disk inventory using `Get-Disk`
- Input validation before high-risk operations
- Confirmation prompts for destructive actions
- DiskPart script generation and execution
- Operational caution around removable or system media

## Important Safety Warning

This script is destructive. Running it against the wrong disk can permanently erase data. Review the script and test only in an isolated lab or disposable virtual machine environment.

Do not run this on a work computer, production endpoint, or personal device unless you fully understand the impact and have verified backups.

## How It Works

1. Lists detected disks and their IDs.
2. Refuses to continue if fewer than two disks are detected.
3. Prompts for the disk ID to sanitize.
4. Prompts for the number of zeroing passes.
5. Requires the user to type `confirm` before continuing.
6. Builds a DiskPart script and runs the sanitation process.

## Production Support Relevance

This project shows comfort with Windows administrative tooling, cautious handling of destructive operations, and operational scripting. Those skills are relevant to support engineering work where clear prompts, guardrails, and validation matter before executing high-impact actions.

## Suggested Improvements

- Add a dry-run mode.
- Add transcript logging.
- Add stronger protection against selecting the system disk.
- Add support for `-WhatIf` and `-Confirm` PowerShell conventions.
