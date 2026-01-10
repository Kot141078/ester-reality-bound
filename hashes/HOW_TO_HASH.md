# How to generate SHA-256 manifests

## Linux / macOS
From the repo root:

```bash
find . -type f \
  -not -path "./.git/*" \
  -not -path "./hashes/SHA256SUMS_v1.2.0.txt" \
  -print0 | sort -z | xargs -0 sha256sum > hashes/SHA256SUMS_v1.2.0.txt

# Verify
sha256sum -c hashes/SHA256SUMS_v1.2.0.txt
```

## Windows (PowerShell)
From the repo root:

```powershell
$files = Get-ChildItem -Recurse -File |
  Where-Object { $_.FullName -notmatch "\\.git\\" -and $_.Name -ne "SHA256SUMS_v1.2.0.txt" } |
  Sort-Object FullName

$lines = foreach ($f in $files) {
  $h = (Get-FileHash $f.FullName -Algorithm SHA256).Hash.ToLower()
  $rel = $f.FullName.Substring((Get-Location).Path.Length + 1).Replace("\\","/")
  "$h  $rel"
}

$lines | Set-Content -Encoding ASCII hashes/SHA256SUMS_v1.2.0.txt
```

Verify by recomputing and comparing.
