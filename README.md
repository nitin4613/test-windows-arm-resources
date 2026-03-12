# Test Windows ARM Resource Classes

Smoke test for CircleCI Windows ARM resource classes.

| Resource Class | CPU | RAM | Credits/min |
|---|---|---|---|
| `windows.arm.medium` | 4 | 16 GB | 40 |
| `windows.arm.large` | 8 | 32 GB | 80 |
| `windows.arm.xlarge` | 16 | 64 GB | 160 |
| `windows.arm.2xlarge` | 32 | 128 GB | 320 |

Each job runs `systeminfo` and `wmic` to verify the provisioned CPU and memory match the expected specs.
