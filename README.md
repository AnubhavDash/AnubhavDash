# Portfolio

![disclosures](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/AnubhavDash/AnubhavDash/main/.github/badge.json)

AI & ML student. Security research on L1 consensus clients and multimedia attack surface.

### Selected disclosures

Every entry is publicly verifiable: each links to a merged fix or a published advisory. Dates are the fix-merge or publication month.

| Date | Project | Severity | Vulnerability | Reference |
|------|---------|----------|---------------|-----------|
| 2026-10 | klever-go | Moderate | Marketplace buy/settlement skips transfer-policy checks, routing restricted balances | [GHSA-3rvr-m2w2-ggqj](https://github.com/klever-io/klever-go/security/advisories/GHSA-3rvr-m2w2-ggqj) |
| 2026-10 | klever-go | Moderate | ITO purchases move a paused/transfer-restricted currency without applying its transfer controls | [GHSA-vjj9-8392-w5hw](https://github.com/klever-io/klever-go/security/advisories/GHSA-vjj9-8392-w5hw) |
| 2026-10 | klever-go | Moderate | FPR deposit and claim paths skip reward-currency transfer policy, routing restricted balances | [GHSA-h45p-mxgj-59f8](https://github.com/klever-io/klever-go/security/advisories/GHSA-h45p-mxgj-59f8) |
| 2026-10 | klever-go | Moderate | Unauthorized minting: staking-claim supply cap adds two int64s without overflow guard | [GHSA-wx97-fhvf-42vg](https://github.com/klever-io/klever-go/security/advisories/GHSA-wx97-fhvf-42vg) |
| 2026-10 | klever-go | Moderate | Missing `IsRoyaltiesChangeStopped` check in `updateRoyaltiesReceiver` permits post-stop rewrite | [GHSA-344r-g6cw-g546](https://github.com/klever-io/klever-go/security/advisories/GHSA-344r-g6cw-g546) |
| 2026-10 | klever-go | Moderate | Missing `IsNFTMetadataChangeStopped` check in `updateMetadataV2` permits post-stop SFT mutation | [GHSA-54v2-fp39-5w66](https://github.com/klever-io/klever-go/security/advisories/GHSA-54v2-fp39-5w66) |
| 2026-10 | klever-go | **High** | Exponential managed-vector clone amplification causes validator/node DoS | [GHSA-qqr9-92pp-89p7](https://github.com/klever-io/klever-go/security/advisories/GHSA-qqr9-92pp-89p7) |
| 2026-10 | klever-go | **High** | `readKDATransfers` clones one buffer per vector entry before unbounded gas charge | [GHSA-3xw3-gjh2-5j94](https://github.com/klever-io/klever-go/security/advisories/GHSA-3xw3-gjh2-5j94) |
| 2026-10 | klever-go | **High** | Exponential `DeletedAccounts` growth in nested output merges causes validator/node DoS | [GHSA-hw69-3fg8-wrmm](https://github.com/klever-io/klever-go/security/advisories/GHSA-hw69-3fg8-wrmm) |
| 2026-10 | klever-go | Moderate | Unbounded bigint handles cause unmetered `PushState` deep clones | [GHSA-gjm9-w2m6-rmp9](https://github.com/klever-io/klever-go/security/advisories/GHSA-gjm9-w2m6-rmp9) |
| 2026-10 | klever-go | **High** | `BigIntShl` result allocation occurs before result-size gas charging | [GHSA-r2gq-244g-h8p2](https://github.com/klever-io/klever-go/security/advisories/GHSA-r2gq-244g-h8p2) |
| 2026-10 | klever-go | Moderate | Exact-divisibility rounding in `DecreaseAll` adds spurious validator penalties | [GHSA-w99g-8m9m-jrf7](https://github.com/klever-io/klever-go/security/advisories/GHSA-w99g-8m9m-jrf7) |
| 2026-10 | klever-go | Low | Validator fee-split float rounding misallocates integer fee units | [GHSA-x5mg-959h-f66v](https://github.com/klever-io/klever-go/security/advisories/GHSA-x5mg-959h-f66v) |
| 2026-09 | klever-go | **High** | Managed-buffer VM hooks allocate/copy attacker-sized data before bounded gas: OOM via `MBufferSetRandom` | [GHSA-cg9c-gcgh-qgc3](https://github.com/klever-io/klever-go/security/advisories/GHSA-cg9c-gcgh-qgc3) |
| 2026-09 | klever-go | **High** | `MBufferGetByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-vxf6-vgpv-822h](https://github.com/klever-io/klever-go/security/advisories/GHSA-vxf6-vgpv-822h) |
| 2026-09 | klever-go | **High** | `MBufferCopyByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-2m22-3m34-2qxf](https://github.com/klever-io/klever-go/security/advisories/GHSA-2m22-3m34-2qxf) |
| 2026-09 | klever-go | **High** | `MBufferSetByteSlice` int32 overflow bypasses bounds check: VM panic burns all caller gas | [GHSA-wjrx-39g9-j97q](https://github.com/klever-io/klever-go/security/advisories/GHSA-wjrx-39g9-j97q) |
| 2026-09 | klever-go | Moderate | Nil current-block-header dereference in `GetAvailableClaim` crashes node via API | [GHSA-g797-9c85-644m](https://github.com/klever-io/klever-go/security/advisories/GHSA-g797-9c85-644m) |
| 2026-09 | klever-go | **High** | Missing read deadline in `directStreamHandler` pins one goroutine per peer stream: DoS | [GHSA-v8j2-98j2-rqv2](https://github.com/klever-io/klever-go/security/advisories/GHSA-v8j2-98j2-rqv2) |
| 2026-02 | FFmpeg | **High** | Heap overflow in `vf_find_rect.c` via `compare()`: out-of-bounds read | [PR #21457](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21457) |
| 2026-02 | FFmpeg | **High** | Heap overflow in `vf_find_rect.c` via `downscale()`: off-by-one heap buffer over-read | [PR #21409](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21409) |
| 2026-02 | FFmpeg | Low | Integer overflow in `scale_eval.c:144` via `ff_scale_adjust_dimensions()`: division by 0 | [PR #21402](https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/21402) |

Upstream credits these reports by name in its release notes and advisory credit records: `@AnubhavDash` is credited on 19 klever-go security advisories across [v1.7.21](https://github.com/klever-io/klever-go/releases/tag/v1.7.21) and [v1.7.22](https://github.com/klever-io/klever-go/releases/tag/v1.7.22).

- **v1.7.21** — 6 advisories credited, plus removal of the unwired `klever-node-auth` path.
- **v1.7.22** — 13 advisories credited, plus 4 accepted fixes shipped without a separate advisory: FPR epoch trim, expired-FPR residual routing, BigInt setter/getter gas ordering, and per-item managed-vector charging.

Additional findings remain under private disclosure or embargo and are added here as fixes ship.

### Research areas

- **L1 consensus & P2P (Go)**: consensus/epoch logic, validator penalties, direct-stream P2P, heartbeat/peer-state, API safety
- **VM & sandbox safety**: managed-buffer gas metering, bigint/managed-vector bounds, integer overflows, gas accounting order
- **Memory corruption (C/C++)**: FFmpeg heap overflows, integer overflows, OOB reads/writes in multimedia codecs

---

*AI & ML student doing security research on L1 consensus clients and multimedia attack surface. I run autonomous auditing pipelines across Go and C codebases. Focus: L1 consensus & P2P, VM/sandbox safety, and memory corruption.*