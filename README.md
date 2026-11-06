# Hi, I'm Fan Yang 👋

I'm a software engineer working on distributed systems, consensus, storage, and infrastructure tooling, primarily in C++, Rust, and Zig.

At [SmartX](https://www.smartx.com/global), I maintain the consensus and metadata modules of [ZBS](https://www.smartx.com/global/smtx-os) and a ZooKeeper fork. My personal projects explore the same foundations, alongside self-hosted services and practical developer tools.

[Blog](https://fuis.top)

## Libraries

| Project | What it does |
| --- | --- |
| [raftz](https://github.com/fanyang89/raftz) | My primary focus: an embeddable Raft consensus library for Zig, with durable WAL, snapshots, and gRPC transport. |
| [grpc-lite](https://github.com/fanyang89/grpc-lite) | A lightweight, streaming-first gRPC runtime for Zig, with C and C++ APIs and bounded backpressure. |
| [kcp-rs](https://github.com/fanyang89/kcp-rs) | A pure Rust KCP implementation with a Sans-I/O core and optional runtime-independent async integration. |
| [lttng-ctl-go](https://github.com/fanyang89/lttng-ctl-go) | Go bindings for liblttng-ctl, with a high-level recording API, complete 2.14 API bindings, and multi-version runtime support. |
| [libclock](https://github.com/fanyang89/libclock) | A C++11 timing library with selectable clock backends, typed timestamps, and stopwatches. |
| [libdns](https://github.com/fanyang89/libdns) | A small Rust DNS server library built on hickory-dns. |
| [gwp-asan](https://github.com/fanyang89/gwp-asan) | Standalone packaging of LLVM's sampled memory-error detector for Linux, with CMake integration. |

Earlier work: [raftpp](https://github.com/fanyang89/raftpp), my C++17 Raft implementation, is planned for archival as development focus shifts to raftz.

## Systems Experiments

- [zookeeper-zig](https://github.com/fanyang89/zookeeper-zig) — A native Zig implementation of ZooKeeper, including protocol codecs, clients, and quorum-server work.
- [Zettide](https://github.com/fanyang89/zettide) — Experimental single-node block storage for VM disks, with a Catalog/Volume engine and local multi-disk protection.
- [nano-vllm-rs](https://github.com/fanyang89/nano-vllm-rs) — A Rust/Burn inference engine for Qwen3-family models, with CPU, CUDA, and ROCm execution paths and inference benchmarks.

## Self-hosted Systems

| Project | What it does |
| --- | --- |
| [qtr](https://github.com/fanyang89/qtr) | QEMU/libvirt virtual machine management with declarative configuration, a CLI, a Web UI, and a REST API. |
| [etz](https://github.com/fanyang89/etz) | Invite-based private networking with end-to-end encryption, TCP hole punching, and subnet routing. |
| [mini-harbor](https://github.com/fanyang89/mini-harbor) | A self-hosted container image registry. |
| [cnb-docker-mirror](https://github.com/fanyang89/cnb-docker-mirror) | Sync container images to CNB and run a local registry mirror backed by a CNB workspace. |
| [plocate-server](https://github.com/fanyang89/plocate-server) | Filename and path search over large file trees, with a plocate index, Web UI, REST API, and MCP tools. |
| [grep-nest](https://github.com/fanyang89/grep-nest) | Code search backed by OpenGrok, accessible through a focused Web UI, REST API, and MCP tools. |
| [service_manager](https://github.com/fanyang89/service_manager) | Cross-platform user-service management through a desktop tray app or a headless Web interface. |
| [services-tray](https://github.com/fanyang89/services-tray) | A Rust service manager with an embedded Web UI, process lifecycle controls, and live logs. |
| [file-desk](https://github.com/fanyang89/file-desk) | A browser-based file manager for local development and internal environments. |

## Developer Tools

### Observability and Diagnostics

- [bpftrace-formatter](https://github.com/fanyang89/bpftrace-formatter) — Formatting and language tooling for bpftrace.
- [prom-cli](https://github.com/fanyang89/prom-cli) — Inspect Prometheus and OpenMetrics endpoints with filtering, live views, and JSON output.
- [ncdu-kv](https://github.com/fanyang89/ncdu-kv) — Find large key prefixes in live ZooKeeper trees or offline ZooKeeper and LevelDB databases.
- [zkctl](https://github.com/fanyang89/zkctl) — Browse and edit ZooKeeper znodes through a shell-like REPL or scripted commands.
- [thermal-cli](https://github.com/fanyang89/thermal-cli) — Linux hardware temperature monitoring with live readings and daemon-mode alerts.
- [many-metrics](https://github.com/fanyang89/many-metrics) — Generate synthetic Prometheus metrics and analyze label combinations.
- [pcap-sherlock](https://github.com/fanyang89/pcap-sherlock) — Analyze TCP anomaly clusters in packet captures and visualize their timing.

### Build and Workflow

- [make-pace](https://github.com/fanyang89/make-pace) — Resource-aware parallel builds.
- [yaml-compose](https://github.com/fanyang89/yaml-compose) — Compose configuration from a base YAML file and ordered layers.
- [git-repo-stash](https://github.com/fanyang89/git-repo-stash) — Discover local Git repositories and back up committed data to Gitea.
- [vibe-sandbox](https://github.com/fanyang89/vibe-sandbox) — Isolated Git worktree and Docker environments for OpenCode workflows.
- [pi-remember-model](https://github.com/fanyang89/pi-remember-model) — A Pi extension that remembers the selected model across new sessions.

### Desktop and File Utilities

- [browser-dispatcher-rs](https://github.com/fanyang89/browser-dispatcher-rs) — Route URLs to different browsers using host and URL rules on Windows, macOS, and Linux.
- [magic-rename](https://github.com/fanyang89/magic-rename) — Detect file contents and correct missing or incorrect extensions.
- [gofd](https://github.com/fanyang89/gofd) — Cross-platform file discovery and management from the command line.
- [keyframe-extract](https://github.com/fanyang89/keyframe-extract) — Select video highlights using semantic relevance, visual quality, and diversity.
- [media-collector](https://github.com/fanyang89/media-collector) — Download Bilibili videos through a command-line workflow.

## Upstream Contributions

Selected merged contributions:

- **EasyTier** — Networking, performance, CLI, and cross-platform improvements, including [packet receive fast paths](https://github.com/EasyTier/EasyTier/pull/2426), [memory reclamation](https://github.com/EasyTier/EasyTier/pull/2428), and [Windows interface caching](https://github.com/EasyTier/EasyTier/pull/2744).
- **lzokay-native-rs** — [Bounded decompression APIs](https://github.com/arma-tools/lzokay-native-rs/pull/2).
- **chdb-go** — [Fix Parquet row handling at the EOF boundary](https://github.com/chdb-io/chdb-go/pull/34).
- **kcp-sys** — [KCP 2.0 API updates](https://github.com/EasyTier/kcp-sys/pull/3) and [RISC-V bindgen support](https://github.com/EasyTier/kcp-sys/pull/4).

<details>
<summary>Recently merged upstream pull requests</summary>

Selected from the past six months, ordered by merge date (newest first).

<!--START_SECTION:activity-->
### arma-tools/lzokay-native-rs
- 🔀 [#2 Add bounded decompression APIs](https://github.com/arma-tools/lzokay-native-rs/pull/2)

### EasyTier/EasyTier
- 🔀 [#2744 perf(common): cache interface snapshots on the Windows bind path](https://github.com/EasyTier/EasyTier/pull/2744)
- 🔀 [#2743 fix(proto): set PROTOC_INCLUDE when sourcing protoc on Windows](https://github.com/EasyTier/EasyTier/pull/2743)

### bytedance/comfyui-lumi-batcher
- 🔀 [#95 feat: 任务列表支持列宽拖拽调整，任务名称列更宽并始终显示完整 tooltip](https://github.com/bytedance/comfyui-lumi-batcher/pull/95)

### EasyTier-Pro/installer
- 🔀 [#1 fix: satisfy clippy warnings](https://github.com/EasyTier-Pro/installer/pull/1)

### zdyxry/tokui
- 🔀 [#9 fix: close preview with q without quitting](https://github.com/zdyxry/tokui/pull/9)
<!--END_SECTION:activity-->

</details>

<details>
<summary>GitHub stats</summary>

[![GitHub stats](https://github-readme-stats-nine-zeta-80.vercel.app/api?username=fanyang89)](https://github.com/anuraghazra/github-readme-stats)

</details>
