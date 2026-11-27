# Sea Power method history

Keel reads these snapshots when it checks code mods built for older game versions. Each file contains method signatures, SHA-256 digests of their IL and metadata, digests of their transitive callers and callees, and direct call edges. The file name is the SHA-256 of the input `Seapower-Scripts.dll`.

| Sea Power build | Source | Methods |
| --- | --- | ---: |
| 0.9.3-261116 | Steam public build 26712472 | 50,704 |

Generate additional snapshots with the script in Keel. Use the full version string from the game log and supply a separate binaries checkout if needed.

```powershell
./tools/snapshot-methods.ps1 -BuildVersion '<full version>' -GameDir '<Sea Power install>' -BinariesRepo '<SEARATS/binaries checkout>'
```

Add new builds alongside existing snapshots. Keep game DLLs and raw IL out of this repository.
