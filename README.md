# Repolex Knowledge Graph of samypr100/backports.asyncio.runner

RDF knowledge graph data for [samypr100/backports.asyncio.runner](https://github.com/samypr100/backports.asyncio.runner), parsed by [repolex](https://repolex.ai).

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
rlex download samypr100/backports.asyncio.runner
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 1d691044f48fae3ae607dcd649c071439204e122
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 1d691044f48fae3ae607dcd649c071439204e122
│           └── chunk-001.nq.gz
├── blob
│   ├── 317d608ee7a210175c289370fc24ee502cde9d8b.nq.gz
│   ├── 4929b25074ba56b0df332da8a2e83744551771a6.nq.gz
│   ├── 4e812ab583178f2eab05a13c3dae36d975233120.nq.gz
│   ├── 5e899f3c4de677796e305ea070d16f162dddb804.nq.gz
│   ├── 6313b56c57848efce05faa7aa7e901ccfc2886ea.nq.gz
│   ├── 65596008fd1a3627ed7d86835c9089f9103140ab.nq.gz
│   ├── 665048fd4a5613132cd7a468574422ccc3dd1d38.nq.gz
│   ├── 73935ad74688989a3ada6227fc6759c9d57608b2.nq.gz
│   ├── 7459f196524ea26f55b8d10cc1466a0625e5a007.nq.gz
│   ├── 7534ac032e7b540d4546bee98b523ae5638ac699.nq.gz
│   ├── 79ec3ce7738b18bb4a66f9efd4c6b32e53d17216.nq.gz
│   ├── 8b1b22152c46d5938296d14e61d01dfd8a433505.nq.gz
│   ├── a0f86ac3c89023eba931a71da8e751e5239ae365.nq.gz
│   ├── b54b535a76bf6ec0ab93066a258b4e416c36d0e8.nq.gz
│   ├── bf216efb1e68ba7f595d0ca0f482cbf1ed2d68a5.nq.gz
│   ├── c210a90a9be5958ae6251818952555ff6fadc56d.nq.gz
│   ├── cbcc22516b8fd246f9a762a7f938e5577c31c6c5.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ed2c4b03932e0f91baac8a17e9bf46ec9827a753.nq.gz
│   ├── f15f0f427964be86e1f94c0d0bec354a7ed1c9b7.nq.gz
│   ├── f7b36b030bdf33d564ea86a1ccb6684cb1977d70.nq.gz
│   ├── f7e7418757817ebe5ca189abeb5a2c25020ba861.nq.gz
│   ├── fce3ef4eaf3c86ee2c95ee5158534e3dd026b6c0.nq.gz
│   └── fff3597592ad419a121b95c22d55fef832982382.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 1d691044f48fae3ae607dcd649c071439204e122.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 30 files
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

[samypr100/backports.asyncio.runner](https://github.com/samypr100/backports.asyncio.runner)

---
*Parsed on 2026-11-02 by [repolex](https://repolex.ai)*
