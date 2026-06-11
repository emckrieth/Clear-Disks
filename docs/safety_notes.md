# Safety Notes

## Risk Level

High. This script performs destructive disk operations through DiskPart.

## Recommended Safeguards

- Run only in a lab environment.
- Verify disk ID, disk name, and disk size before confirming.
- Never test against production endpoints or personal devices with important data.
- Keep backups before any disk sanitation activity.
- Prefer a dry-run mode before executing destructive commands.

## Support Engineering Takeaway

For production support, high-impact tools should include explicit confirmation, strong validation, clear logging, and rollback or recovery planning where possible.
