# entreprise-infrastructure-lab-
## SGID Configuration

Applied SGID to the shared directory:

```bash
sudo chmod 2770 /company/IT
```

Verified directory permissions:

`drwxrws---`

## SGID Test

Created a file as Ahmed:

```bash
sudo -u ahmed touch /company/IT/test-ahmed.txt
```

Verified file ownership:

`-rw-r--r-- 1 ahmed IT ... test-ahmed.txt`

Result: The new file automatically inherited the IT group.

**Status: Successful**
