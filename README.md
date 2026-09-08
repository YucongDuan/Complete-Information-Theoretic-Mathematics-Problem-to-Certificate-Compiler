# DIKWP-CITM Forge

Created by Yucong Duan (段玉聪).

[Quick start / 快速开始](#quick-start--快速开始) · [Core outputs / 核心输出](#core-outputs--核心输出) · [Download the release package / 下载发布包](./DIKWP-CITM-Forge-v1.0.0.zip)

> Release layout / 发布结构 — The runnable source is distributed in `DIKWP-CITM-Forge-v1.0.0.zip`. Extract it first; the commands below assume that you have entered the extracted `DIKWP-CITM-Forge-v1.0.0` directory. / 可运行源码位于上述 ZIP 发布包中；请先解压。下方命令默认已经进入解压后的 `DIKWP-CITM-Forge-v1.0.0` 目录。

Complete Information-Theoretic Mathematics Problem-to-Certificate Compiler  
完全信息理论数学：问题—证书编译与审计系统

DIKWP-CITM Forge converts a declared mathematical problem into a deterministic, hash-linked, machine-readable audit package. It combines finite information-theory calculations, future-effect quotients, plural world models, D/I/K/W/P record constellations, twenty-five record-level route kinds, proof obligations, and a strict reduction firewall.

The system is deliberately non-sovereign. It can verify a finite table, a declarative witness, a hash chain, a local quotient, or a protocol invariant. It cannot silently convert any of those achievements into an unrestricted theorem, external mathematical acceptance, empirical truth, life, or phenomenal consciousness.

DIKWP-CITM Forge 将数学问题编译为确定性、哈希链接、机器可读的审计包。系统同时实现有限信息论计算、未来同效商、多世界模型、D/I/K/W/P 多记录结构、二十五类记录级路径、证明义务和“还原不等于证明”防火墙。

系统只签发其实际验证范围内的证书。有限计算、局部结构、术语重述、问题还原或软件测试均不会被静默升级为无界全称定理或外部领域最终结论。

## Core outputs / 核心输出

Each compile produces:

- `normalized_project.json` — canonical input object;
- `ledger.jsonl` — nine-stage append-only hash chain;
- `audit.json` — complete non-aggregated audit;
- `certificate.json` — scope-bounded certificate;
- `audit_report.md` — bilingual human-readable report;
- `dashboard_data.json` — offline dashboard payload;
- `output_manifest.json` — per-file SHA-256 and Merkle root.

## Quick start / 快速开始

No third-party runtime dependency is required.

```bash
cd DIKWP-CITM-Forge-v1.0.0
export PYTHONPATH="$PWD/src"       # Windows: set PYTHONPATH=%CD%\src
python -m citm_forge demo --output outputs/demo
python -m citm_forge verify-ledger outputs/demo/ledger.jsonl
python -m citm_forge show-status outputs/demo/certificate.json
```

Or install locally:

```bash
python -m pip install .
citm-forge demo --output outputs/demo
```

Open `web/DIKWP_CITM_Forge_Offline_Demo.html` directly in a browser. The dashboard has no external script, font, image, analytics, network, or model dependency.

## Compile a project / 编译项目

```bash
python -m citm_forge compile examples/05_goldbach_finite/project.json \
  --output outputs/goldbach-finite
```

The included Goldbach example verifies only the declared finite range. Its certificate explicitly refuses the requested unrestricted `SOLVED` status.
