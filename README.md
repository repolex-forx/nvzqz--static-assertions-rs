# Repolex Knowledge Graph of nvzqz/static-assertions-rs

RDF knowledge graph data for [nvzqz/static-assertions-rs](https://github.com/nvzqz/static-assertions-rs), parsed by [repolex](https://repolex.ai).

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
rlex download nvzqz/static-assertions-rs
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 18bc65a094d890fe1faa5d3ccb70f12b89eabf56
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 18bc65a094d890fe1faa5d3ccb70f12b89eabf56.nq.gz
│   └── repolex
│       └── 18bc65a094d890fe1faa5d3ccb70f12b89eabf56
│           └── chunk-001.nq.gz
├── blob
│   ├── 00f624277554913c78ee35c402f25284ae7afe02.nq.gz
│   ├── 03a26f5686685ef71e969915ccc4f603ab897f48.nq.gz
│   ├── 16ae4a6b42d969ece2333374e3789a1e1846168e.nq.gz
│   ├── 22c6248d5eee46136a612d58f12dbd9f2c469723.nq.gz
│   ├── 24282c1f32b53d6f8b6dd96d8e73787affe5076b.nq.gz
│   ├── 30248fce2a4a6887c4c95bbe12864deaf281555a.nq.gz
│   ├── 3adfef079c825d73c390f7cbb8bfb614f0e3ea89.nq.gz
│   ├── 480b6b6c61a8834c47cfd68c46333de3efc19d87.nq.gz
│   ├── 69412daefb62f895680343b6aa8fca0c4f075276.nq.gz
│   ├── 70e89d59591857f406e915983bb7581cf9f5f08b.nq.gz
│   ├── 74bdb2fc308e8a24a607ce88eaddfbd5aeaa1b4b.nq.gz
│   ├── 7638d66671c97a9e38357814af8f8e4b54fcd2cc.nq.gz
│   ├── 80d55075fc43d4220bf5726e441cefc0e555d139.nq.gz
│   ├── 97847b26f95ed9e738f71f85f297ed71ba2e402a.nq.gz
│   ├── 9c3c4901c7cbbddea4f2bf3ab9e8db3ec810cac2.nq.gz
│   ├── a43cc1f56d9fc39001779394bc8c85cf6500798b.nq.gz
│   ├── aa4e6f51c0a11ff72db278bf05e1be6e1d217831.nq.gz
│   ├── bca222ed558affef501d2d96de51982e2c93b892.nq.gz
│   ├── c231492fda60e2e3e0b6fb9df8352190b4790a29.nq.gz
│   ├── ccc94459f8ed9ec43bce6f8aa6bd59072b82890e.nq.gz
│   ├── cdd2d70929c9c374323caa1b08f32c7acd74daa8.nq.gz
│   ├── d645695673349e3947e8e5ae42332d0ac3164cd7.nq.gz
│   ├── dd2dc2a6f7bb311a63b13b75794abb1c36c8e567.nq.gz
│   ├── ecbba96475857af47d6f687d486caba775cd6141.nq.gz
│   └── f1f90304f28182bfc7c0f0e2479f6155d8141b5f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 18bc65a094d890fe1faa5d3ccb70f12b89eabf56.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 34 files
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

[nvzqz/static-assertions-rs](https://github.com/nvzqz/static-assertions-rs)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
