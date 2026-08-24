# DIKWP-CITM Forge

**Complete Information-Theoretic Mathematics Problem-to-Certificate Compiler**  
**完全信息理论数学：问题—证书编译与审计系统**

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

## Nine-stage pipeline / 九阶段账本

1. Normalised specification / 规范化规格
2. Claim replay / 主张重放
3. Carrier audit / 载体审计
4. Pattern and route audit / 母式与路径审计
5. Semantic decompression / 语义解压
6. Quantifier audit / 量词审计
7. Eight-dimensional bridge / 八维桥接
8. Maximum persistent core / 最大持续核心
9. Non-aggregated settlement / 非聚合结算

## Mathematical runtime / 数学运行时

The dependency-free runtime includes:

- finite Shannon entropy and mutual information;
- finite channel composition and data-processing audit;
- finite Bayes-risk and decision-sufficiency audit;
- future-effect equivalence quotient and monotone refinement;
- typed route graph over D/I/K/W/P;
- W-to-forward-P visibility and explicit P-to-output paths;
- forward-P → candidate-K → reverse-P → regenerated-output → D-sameness round trips;
- non-isomorphic world-model comparison and reversible authorised probe ranking;
- safe declarative finite verifiers;
- reduction soundness/completeness/target-obligation firewall;
- deterministic replay, SHA-256 chain, file manifest, and Merkle root.

## Status vocabulary / 状态词汇

The runtime uses bounded statuses such as:

- `PROTOCOL_VALID`
- `VERIFIED_WITHIN_DECLARED_SCOPE`
- `EQUIVALENCE_VERIFIED_WITHIN_DECLARED_SCOPE`
- `REDUCTION_ONLY`
- `OPEN`
- `NOT_ESTABLISHED`
- `REFUSED_OVERCLAIM`
- `FAILED`

It does not issue `FINAL_TRUTH` or a global theorem verdict from an internal run.

## Open-problem registers / 未解问题登记

`examples/open_problems/` contains explicit, non-solution registers for:

- Strong Goldbach;
- P versus NP;
- Riemann Hypothesis;
- Birch–Swinnerton-Dyer;
- Hodge;
- Navier–Stokes existence and smoothness;
- Yang–Mills existence and mass gap.

Each retains the inherited object domain and external settlement standard. These examples show how to preserve proof obligations without pretending that an information-theoretic reduction is already the missing proof.

## Security boundary / 安全边界

- project files are declarative JSON;
- no project-supplied Python, shell, solver, plugin, network call, credential, or physical action is executed;
- automatic external-action authority is always `0`;
- a probe can be ranked only when it is declared, reversible, and names its authorising principal;
- ranking is not execution;
- the local static server is read-only and binds to `127.0.0.1` by default.

## Authorship and licensing / 署名与许可

The theoretical source is the bilingual book *A New Mathematical History of the Universe* / 《宇宙的数学新史》 by **Yucong Duan and Feng Wang**. The release preserves source lineage, authorship, limitations, and non-impersonation boundaries.

- Runtime code: **AGPL-3.0-or-later**
- Schemas and conformance interfaces: **Apache-2.0**
- Documentation and examples: **CC BY 4.0**

See `NOTICE`, `AUTHORS.md`, `LICENSE_POLICY.md`, and `licenses/`.

## Reproducibility / 可复现性

```bash
./run_tests.sh
./run_demo.sh
python scripts/verify_release.py
```

The reference run and release manifest are generated locally. No GitHub publication, DOI, signature, institutional endorsement, or external acceptance is claimed by this package.
