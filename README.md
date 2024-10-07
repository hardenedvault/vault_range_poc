# Vault Range PoC
Project Vault Range PoC: Know your enemy and yourself to build better defense-in-depth solution! HardenedVault will share some of technical experience we gained during the daily work of building open source based security solution for platform/infrastructure, e.g: Linux kernel, firmware and cryptography engineering. 

Any contributors are welcomed as well!


## Proof of Concepts

Proof-of-concept/exploit code will be used to demonstrate the security vulnerabilities. Do not tweak them in the production.

## Write-up

 * [Vault Range - The Measure and Resilience of Weaponized Exploit Methods for Linux - updating](https://hardenedvault.net/blog/2023-07-16-vault-range-resilience-weaponized-exp-linux/)
 * [Exploiting CVE-2021-26708 (Linux kernel) with sshd - 202203](https://hardenedvault.net/2022/03/01/poc-cve-2021-26708.html)

## Exploit methods
| Vulnerability | Exploitation techniques | Can VED mitigate? |
|:-------------:|:-----------------------:|:-----------------:|
|CVE-2021-22555 | Bypass CONFIG_SLAB_FREELIST_HARDENED/KASLR/SMAP + ROP| YES |
|CVE-2021-22555 | ++ with bypass Tetragon | Yes |
|CVE-2021-22555 | ++ with pipe-primitive  | Yes |
|CVE-2022-2639  | Random object to heap straying with  pipe-primitive | Yes |
|CVE-2022-34918 | Heap ***                | Yes |
|CVE-2022-0847  | Dirty Pipe              | No |
|Any            | [SLUBStick](https://hardenedvault.net/blog/2024-08-25-slubstick-risk-assessment-embedded-system/)               | Partially |

## Licence

All PoC/exploit in Vault Range PoC are under GPLv3. See [LICENSE](https://github.com/hardenedvault/vault_range_poc/blob/master/LICENSE) for
further details.


