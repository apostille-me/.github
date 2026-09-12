# Complete local Git recovery archive — apostille-me

This archive preserves every discovered local Git ref and dirty worktree patch for `apostille-me` before semantic reconciliation. Current canonical branches remain authoritative; no force-push or default-branch mutation is implied.

Restore:

```bash
cat apostille-me-git-recovery-2026-08-09.tar.gz.b64.part* | base64 --decode > apostille-me-git-recovery-2026-08-09.tar.gz
sha256sum apostille-me-git-recovery-2026-08-09.tar.gz
tar -xzf apostille-me-git-recovery-2026-08-09.tar.gz
```

Compare archived refs semantically against current canonical history before porting them.
