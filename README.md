# Portfolio

![disclosures](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/AnubhavDash/AnubhavDash/main/.github/badge.json)

Security researcher working on L1 nodes and multimedia attack surface. I run auditing pipelines across Go and C codebases. Focus: P2P networking, VM/sandbox safety, and memory corruption.

### Selected disclosures

Every entry is publicly verifiable: each links to a merged fix or a published advisory. Dates are the fix-merge or publication month.

| Date | Project | Severity | Vulnerability | Reference |
|------|---------|----------|---------------|-----------|
| 2026-10 | klever-go | Moderate | Marketplace Buy and Settlement Move Order Currency Without Transfer-Policy Checks, Routing Restricted Balances | [GHSA-3rvr-m2w2-ggqj](https://github.com/klever-io/klever-go/security/advisories/GHSA-3rvr-m2w2-ggqj) |
| 2026-10 | klever-go | Moderate | ITO purchases move a paused or transfer-restricted currency without applying its transfer controls | [GHSA-vjj9-8392-w5hw](https://github.com/klever-io/klever-go/security/advisories/GHSA-vjj9-8392-w5hw) |
| 2026-10 | klever-go | Moderate | FPR Deposit and Claim Paths Skip Reward-Currency Transfer Policy, Routing Restricted Balances | [GHSA-h45p-mxgj-59f8](https://github.com/klever-io/klever-go/security/advisories/GHSA-h45p-mxgj-59f8) |
| 2026-10 | klever-go | Moderate | Unauthorized minting: the staking-claim supply cap adds two int64s without an overflow guard, so a LARGER mint is accepted where a smaller one is refused | [GHSA-wx97-fhvf-42vg](https://github.com/klever-io/klever-go/security/advisories/GHSA-wx97-fhvf-42vg) |
| 2026-10 | klever-go | Moderate | Missing IsRoyaltiesChangeStopped Check in updateRoyaltiesReceiver Permits Post-Stop Royalties Receiver Rewrite | [GHSA-344r-g6cw-g546](https://github.com/klever-io/klever-go/security/advisories/GHSA-344r-g6cw-g546) |
| 2026-10 | klever-go | Moderate | Missing IsNFTMetadataChangeStopped Check in updateMetadataV2 Permits Post-Stop SFT Metadata Mutation | [GHSA-54v2-fp39-5w66](https://github.com/klever-io/klever-go/security/advisories/GHSA-54v2-fp39-5w66) |
| 2026-10 | klever-go | **High** | Exponential Managed-Vector Clone Amplification Causes Validator/Node Denial of Service | [GHSA-qqr9-92pp-89p7](https://github.com/klever-io/klever-go/security/advisories/GHSA-qqr9-92pp-89p7) |
| 2026-10 | klever-go | **High** | readKDATransfers clones one buffer per vector entry before unbounded gas charge, enabling remote memory exhaustion | [GHSA-3xw3-gjh2-5j94](https://github.com/klever-io/klever-go/security/advisories/GHSA-3xw3-gjh2-5j94) |
| 2026-10 | klever-go | **High** | Exponential DeletedAccounts growth in nested output merges causes validator/node denial of service | [GHSA-hw69-3fg8-wrmm](https://github.com/klever-io/klever-go/security/advisories/GHSA-hw69-3fg8-wrmm) |
| 2026-10 | klever-go | Moderate | Unbounded bigint handles cause unmetered `PushState` deep clones | [GHSA-gjm9-w2m6-rmp9](https://github.com/klever-io/klever-go/security/advisories/GHSA-gjm9-w2m6-rmp9) |
| 2026-10 | klever-go | **High** | `BigIntShl` result allocation occurs before result-size gas charging | [GHSA-r2gq-244g-h8p2](https://github.com/klever-io/klever-go/security/advisories/GHSA-r2gq-244g-h8p2) |
| 2026-10 | klever-go | Moderate | Exact-Divisibility Rounding in DecreaseAll Adds Spurious Validator Penalties | [GHSA-w99g-8m9m-jrf7](https://github.com/klever-io/klever-go/security/advisories/GHSA-w99g-8m9m-jrf7) |
| 2026-10 | klever-go | Low | Validator Fee-Split Float Rounding Misallocates Integer Fee Units | [GHSA-x5mg-959h-f66v](https://github.com/klever-io/klever-go/security/advisories/GHSA-x5mg-959h-f66v) |
| 2026-09 | klever-go | **High** | Managed-buffer VM hooks allocate and copy attacker-sized data before bounded gas is enforced: validator memory exhaustion / OOM via `MBufferSetRandom` | [GHSA-cg9c-gcgh-qgc3](https://github.com/klever-io/klever-go/security/advisories/GHSA-cg9c-gcgh-qgc3) |
| 2026-09 | klever-go | **High** | `MBufferGetByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-vxf6-vgpv-822h](https://github.com/klever-io/klever-go/security/advisories/GHSA-vxf6-vgpv-822h) |
| 2026-09 | klever-go | **High** | `MBufferCopyByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-2m22-3m34-2qxf](https://github.com/klever-io/klever-go/security/advisories/GHSA-2m22-3m34-2qxf) |
| 2026-09 | klever-go | **High** | `MBufferSetByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-wjrx-39g9-j97q](https://github.com/klever-io/klever-go/security/advisories/GHSA-wjrx-39g9-j97q) |
| 2026-09 | klever-go | Moderate | Nil current-block-header dereference in `GetAvailableClaim` crashes node via `/address/{address}/allowance/list` | [GHSA-g797-9c85-644m](https://github.com/klever-io/klever-go/security/advisories/GHSA-g797-9c85-644m) |
| 2026-09 | klever-go | **High** | Missing read deadline in `directStreamHandler` pins one goroutine per peer stream: resource exhaustion / DoS | [GHSA-v8j2-98j2-rqv2](https://github.com/klever-io/klever-go/security/advisories/GHSA-v8j2-98j2-rqv2) |
| 2026-02 | FFmpeg | **High** | Heap overflow in `vf_find_rect.c` via `compare()`: out-of-bounds read | [PR #21457](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21457) |
| 2026-02 | FFmpeg | **High** | Heap overflow in `vf_find_rect.c` via `downscale()`: off-by-one heap buffer over-read | [PR #21409](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21409) |
| 2026-02 | FFmpeg | Low | Integer overflow in `scale_eval.c:144` via `ff_scale_adjust_dimensions()`: division by 0 in `eval_expr()` | [PR #21402](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21402) |

Additional findings remain under private disclosure or embargo and are added here as fixes ship.

### Research areas

- L1 and P2P clients (Go): resource exhaustion, pre-auth DoS, node crashes, API safety
- VM and sandbox safety: integer overflows, bounds checks, gas accounting
- Multimedia (C): memory corruption, OOB reads/writes, integer overflows
