# random6

Cybersecurity-focused systems programmer working with Rust, C, Linux kernel, eBPF, and low-level security. Former CTF player.

## Open Source Contributions

Linux kernel BPF contributor.

- **[BPF verifier patch landed in `bpf-next`](https://rust.random6.xyz/blog/linux-kernel-ebpf-verifier-patch-1/)** ([upstream patch](https://lore.kernel.org/all/20260625-bpf-stack-var-off-zero-v1-v3-0-a068210a761b@gmail.com/)) — Refined the verifier's handling of zero stack-variable offsets to reduce excessive conservatism in stack analysis.
- Upstreamed a [`bpftool` flow dissector query error-handling fix](https://lore.kernel.org/all/20260603003339.33791-1-random6.xyz@gmail.com/), replacing fragile `errno`-based logic with libbpf-returned error codes.
- Added and upstreamed a [BPF selftest](https://lore.kernel.org/all/20260612-arena-direct-value-v1-v4-1-b81b642f5277@gmail.com/) covering arena direct-value behavior.

## Projects

A selection of my projects is below. More projects and experiments are available on [GitHub](https://github.com/random6-xyz).

### [rand-verifier](https://github.com/random6-xyz/rand-verifier)

A Rust implementation of the Linux eBPF verifier focused on differential testing and bug discovery.

- **[rand-guard](https://github.com/random6-xyz/rand-guard)** — Rust + Aya EDR
- **[ebpf-guard](https://github.com/random6-xyz/ebpf-guard)** — C-based EDR

## Writing

Selected writing on Linux kernel and eBPF research. More articles and project write-ups are available on [my blog](https://rust.random6.xyz/).

- [eBPF verifier experiments](https://rust.random6.xyz/blog/linux-kernel-ebpf-verifier-experiments/)
- [Partial initialization in the eBPF verifier](https://rust.random6.xyz/blog/linux-kernel-ebpf-partial-init-verifier/)
- [Finding bugs in the eBPF verifier](https://rust.random6.xyz/blog/linux-kernel-ebpf-finding-bug-2/)
- [eBPF selftests and packet access](https://rust.random6.xyz/blog/linux-kernel-ebpf-selftests-pkt-access/)

## Background

- DEF CON 33 Finalist
