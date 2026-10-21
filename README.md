# Repolex Knowledge Graph of executablebooks/mdformat-footnote

RDF knowledge graph data for [executablebooks/mdformat-footnote](https://github.com/executablebooks/mdformat-footnote), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download executablebooks/mdformat-footnote
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9a174e4cba089f4b117134a220164bdc20f070fe
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9a174e4cba089f4b117134a220164bdc20f070fe
│           └── chunk-001.nq.gz
├── blob
│   ├── 0de68f93cd86ac35d4ddcc074c157393341f29c1.nq.gz
│   ├── 223838a01cb4c24bd0dce7c1d83e69faea88bb04.nq.gz
│   ├── 2b1c938fb6f449d69c0608c2c2a7f9e547028595.nq.gz
│   ├── 2efc5d8243d5f5a0e56b17db8ac6a4b12cd4e5e3.nq.gz
│   ├── 49fc30721c8f849964b06f3900ce582523b68c15.nq.gz
│   ├── 4ce065b2b794babb67096df481e4eed5b97bc827.nq.gz
│   ├── 523411b8c1ff266d4cf961b57f68138711907ac2.nq.gz
│   ├── 5768d27dc4647aff882658edd67b3bc44bf65820.nq.gz
│   ├── 668d01d653aea5e90585ef24c1c2c7752d351d67.nq.gz
│   ├── 6afdf312447e05c180b6ef6d8c1675fdddccca08.nq.gz
│   ├── 71c1bbf91003349c8a5b76e20c11f0197ff3ffab.nq.gz
│   ├── 8d9f770ae98c7f2443c98352d62aff95c0bf0b40.nq.gz
│   ├── 8f37780bff8509085cc74c1b437984c9397f6f6b.nq.gz
│   ├── 9643a4ea975e7182c548e4bc8e94accb93aa0056.nq.gz
│   ├── 994653111f7abfd53b8e4e0f932a1696dcf87189.nq.gz
│   ├── 9e9a26d297ad4f2efd384e969e2fa55ad661dcd3.nq.gz
│   ├── a3a0ac02883a36432daaf16e00073bb34bbe0a11.nq.gz
│   ├── a3d36520548d8d65d983e58dcf45a8b7644a68a7.nq.gz
│   ├── b1afc887fcd22484816d4265275a915421ce5df0.nq.gz
│   ├── ea52cb82e2146a0f0206d07b2d0aa21132b59fa1.nq.gz
│   ├── eed4a78b19438dec1ea47360d377f880a345de19.nq.gz
│   ├── fb806b6d03e33507057072ce5ac0981d0de030e6.nq.gz
│   └── fede2f8f20eed91bf818b850cbfe5b4fc6165882.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 9a174e4cba089f4b117134a220164bdc20f070fe.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 31 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[executablebooks/mdformat-footnote](https://github.com/executablebooks/mdformat-footnote)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
