# disable_aslr

## _Disable ASLR with PongoOS_

---

## IMPORTANT

- **The current offset is only for iOS 14.8 iPhone X, you must adjust to use.**
- This can and should be improved using kpf, but i do not have the time to invest into it.

---

## Explanation

- By patching slide to 0 in function [parse_machfile](https://github.com/apple-oss-distributions/xnu/blob/8d741a5de7ff4191bf97d57b9f54c2f6d4a15585/bsd/kern/mach_loader.c#L892) found in the xnu kernel.

---

## Usage (See Makefile for test command)

---

## Credits

- Special thanks to the Checkra1n team for [PongoOS](https://github.com/checkra1n/PongoOS).
- [Billy Ellis](https://github.com/Billy-Ellis) for his [research](https://bellis1000.medium.com/aslr-the-ios-kernel-how-virtual-address-spaces-are-randomised-d76d14dc7ebb).
- [Cryptiiiic](https://github.com/cryptiiiic) for his advice.
- [blacktop](https://github.com/blacktop) for his awesome [ipsw](https://github.com/blacktop/ipsw) tool.
