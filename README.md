# random6 (Woojin Ji)

Systems programmer focused on Linux kernel and eBPF security, working with Rust, C, and Python. Former CTF player.

[Blog](https://rust.random6.xyz/) · [Email](mailto:random6.xyz@gmail.com)

## Open Source Contributions

Linux kernel BPF contributor — four commits in mainline Linux and two merged into `bpf-next`.

- **BPF verifier:** [Preserved known-zero stack reads across scalar zero spills](https://github.com/torvalds/linux/commit/69fdbe63e16919a885a8f9441e248ce0ddf15b25), with spill-precision tracking for sound pruning and [regression selftests](https://github.com/torvalds/linux/commit/e693da913d2cdd69c1612fbf71bdf2b6771f6dba).
- **BPF helper inlining (`bpf-next`):** [Fixed `bpf_get_func_arg()` index zero-extension](https://github.com/torvalds/linux/commit/1c1dda9ba9f3af9cd511a197dcc86de2465d8fe5) to prevent out-of-bounds context reads, with [regression selftests](https://github.com/torvalds/linux/commit/38dbc3047a2fa706f6b4485679eb5eb62ff55b87).
- **BPF selftests:** Added an [arena direct-value regression test](https://github.com/torvalds/linux/commit/7bfb93e3475be9de894f1cecd3a727d3e1649b03) for a one-past-end offset.
- **bpftool:** [Fixed flow-dissector query error handling](https://github.com/torvalds/linux/commit/8a7f2bff2165e53595d1e91c160b340f978c0ab7) to use libbpf's error code instead of `errno` after `close()`, preserving old-kernel compatibility.

## Projects

A selection of my projects is below. More projects and experiments are available on [GitHub](https://github.com/random6-xyz).

### [rand-verifier](https://github.com/random6-xyz/rand-verifier)

Differential testing for the Linux eBPF verifier in Rust, combining abstract interpretation, bounded concrete execution, an independent safety specification, and real-kernel verdicts. Includes fuzzing, test-case reduction, and SMT checks.

- **[kernel-ebpf-lab](https://github.com/random6-xyz/kernel-ebpf-lab)** — Reproducible Buildroot/QEMU kernel environments for BPF patch work and verifier testing.
- **[rand-guard](https://github.com/random6-xyz/rand-guard)** — Rust + Aya endpoint detection prototype with eBPF telemetry, userspace enrichment, and focused detections.

## Writing

Selected writing on Linux kernel and eBPF research. More articles and project write-ups are available on [my blog](https://rust.random6.xyz/).

- [Patching the eBPF Verifier to Preserve Spilled Zeroes](https://rust.random6.xyz/blog/linux-kernel-ebpf-verifier-patch-1/)
- [Why 12 eBPF Partial-Init Variants That Looked Equivalent Produced Different Verification Results](https://rust.random6.xyz/blog/linux-kernel-ebpf-partial-init-verifier/)

## Background

- **DEF CON 33 CTF Finals (2025)** — Finalist with **cold fusion**; pwn and reverse engineering.
- **Dankook University, Jukjeon Campus** — B.Eng. in Cybersecurity, expected February 2028.
