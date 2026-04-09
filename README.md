# Repolex Knowledge Graph of apache/jena

RDF knowledge graph data for [apache/jena](https://github.com/apache/jena), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download apache/jena
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 1b767c8830220f55dcd760e94c0dadf597b6eea4
│   │       ├── chunk-001.nq.gz
│   │       ├── chunk-002.nq.gz
│   │       ├── chunk-003.nq.gz
│   │       ├── chunk-004.nq.gz
│   │       ├── chunk-005.nq.gz
│   │       ├── chunk-006.nq.gz
│   │       └── chunk-007.nq.gz
│   ├── lsp
│   │   └── 1b767c8830220f55dcd760e94c0dadf597b6eea4.nq.gz
│   └── repolex
│       └── 1b767c8830220f55dcd760e94c0dadf597b6eea4
│           ├── chunk-001.nq.gz
│           └── chunk-002.nq.gz
└── blob
    ├── 000114bc4165b9f024c76b55bfa7e02d2af250ea.nq.gz
    ├── 000579ba07ccb2fa11d94eb5573a43de90a6d55b.nq.gz
    ├── 0007a909030addcc57c456b4a1a41c13c7c72584.nq.gz
    ├── 000c234c60ebbbdf6f56fdd56da0bdd7de77c457.nq.gz
    ├── 000c63e9ef9bbe832500ae601497def697b29e49.nq.gz
    ├── 000e32f75fb39fb2cc5be9dc6b0b4e06f800ab04.nq.gz
    ├── 000fd1cb88cedb071c427001400d96467bd06a47.nq.gz
    ├── 0012db33c7b63444844dd2d5ba86d67e623e6a7c.nq.gz
    ├── 001323a48add5bf77638eeb5508d7526ebabd445.nq.gz
    ├── 0016cda3c8bd77ae84c169f47541722b97beddbb.nq.gz
    ├── 00295822de4d35d5b93886603313abbd84cd0801.nq.gz
    ├── 002a18a045338bb6a124a964b5f72be331d12d2e.nq.gz
    ├── 002c828b3947cd541b52065d10318150e0734ff5.nq.gz
    ├── 002e5ee01a0b53d9661b54a976479b2bbb7af4d6.nq.gz
    ├── 003663d17e8632d0f7b1af19ba5deaf69b72ee81.nq.gz
    ├── 004360483051d74f56917e9c39e5d3c3a3a07a63.nq.gz
    ├── 005990be22fbab71bcbe0fd9891011d4cd435ab6.nq.gz
    ├── 006d8edecbb685ab2b273a0c2aafaca9d645d73e.nq.gz
    ├── 0079ff1dd58a929042f9a4e89f89a12abbcc55f7.nq.gz
    ├── 0081b1a27333d48417b7fedc39ef4f69da8e685b.nq.gz
    ├── 009681cc74b15538d203dcc2c29f9bd2eb737331.nq.gz
    ├── 0098738d329b83cefbe8e7fee78826bd3031db8a.nq.gz
    ├── 00988b53f57ef1db8a7ebfae47f52ae801564321.nq.gz
    ├── 009e038cfb5f7190244c9214dfcc04385733127c.nq.gz
    ├── 009ea06d5084a3b38dc34890d07125f5b5a6f47c.nq.gz
    ├── 00ab03d01672695fc5cabf0ad93488bb04723595.nq.gz
    ├── 00c191e156e031a124976ccdb97aafad892f5d7e.nq.gz
    ├── 00c96817199d3d9e47cc30d39aac9ef3d963db8a.nq.gz
    ├── 00caa33572ac2a0fa79ab985c0876daa5943d4ed.nq.gz
    ├── 00d43d84add80c3c1b574810ee501e9eaa94ed9c.nq.gz
    ├── 00d6f9cced317fa9486177c05bc9cf2a8a49d1b4.nq.gz
    ├── 00e92a5ecba20c973eddc6f2b26ef5f05b6acd02.nq.gz
    ├── 00ec569ae8e5555f219001cd5341b96fde9833f2.nq.gz
    ├── 00f1529016d4f05eb12a916e0f53b66ae9ab9cd3.nq.gz
    ├── 00f1bcb6ad54c1b5c32711832652ff1d3b63b1f2.nq.gz
    ├── 00f2806c1d641599043a70c3b66d9b717822845a.nq.gz
    ├── 00f6c798f36315c9daa14b046c39579391709e97.nq.gz
    ├── 00f9e32dfc4e6bc76e622d13702d3e0f2a7252a4.nq.gz
    ├── 0100e862b2cbfd3dbdc5710489c94b34ac55bf75.nq.gz
    ├── 010a7b722ddfe2431af344c515b40686f297ffa8.nq.gz
    ├── 010cad44997c60c569211b040b73f5acd96d09d4.nq.gz
    ├── 0114391c252c1ce25b0fa6a8905d9e21179fbe18.nq.gz
    ├── 0122cf3778d94cb023d2a9cb405d1b09a5a747ee.nq.gz
    ├── 0128761d9cc18276c20a63299eb8b37d6b52cf8b.nq.gz
    ├── 012e24a070e21f54ea2b7f3c1c5b8305c5ff0eeb.nq.gz
    ├── 01345467b018acc80ec01026c63cc80ea1a7de47.nq.gz
    ├── 014afcc4896a3eac9dc41f062d00344349692bb6.nq.gz
    ├── 014e177ab62320b00d3ad57710588c4dd21a3fbd.nq.gz
    ├── 015a315a58c37324f4fc661df0676e8a77f13bff.nq.gz
    ├── 015c3c70f0edb544365dd9a2523156090037b696.nq.gz
    ├── 015c99c8f838a0ca5f31cf0711ebce29727c0448.nq.gz
    ├── 0164e336a928157214557d471abcb75e10c564d4.nq.gz
    ├── 01751af0e3220ba853b1cafcea69642943ec5216.nq.gz
    ├── 017cf7d873e3e83ca39c6f43cdfc3c4771b48b1c.nq.gz
    ├── 017e44f440c0c3df780046bad9c0d3f6bc30c35d.nq.gz
    ├── 0181d7282ae9228fe3496cd480b1752323f69598.nq.gz
    ├── 0187d7ad5085101daa33390a955e0138a1c9a72b.nq.gz
    ├── 018ce254c456f9f4baabeebcba309ec8134b0dea.nq.gz
    ├── 0192047f776c866738ce0c8d797b492a675bf9ce.nq.gz
    ├── 019d697bb63e3484f04040296631c808f74dfe68.nq.gz
    ├── 01a0aec2ba60d1ff6ebaf318fb19d29123370fb5.nq.gz
    ├── 01bdf0f87c092c42e1b8982ec0f951e88c6db5f3.nq.gz
    ├── 01c4966ce546aff208bb4cd8a81fe23a77ba8dae.nq.gz
    ├── 01d095e34cebba0c0c0c3df7cd30a615e873e35a.nq.gz
    ├── 01ee030ca07b2cd2cca785391b5c86077e14d6f0.nq.gz
    ├── 01f7935a539f1a76e597c208fdc092e1d8971156.nq.gz
    ├── 020c6413313a1f4997a61958e4083f4989177580.nq.gz
    ├── 020e232e2c21eafe66a0486c303aabbd83712965.nq.gz
    ├── 0212f362463d27851c400c119637c9171d7abb58.nq.gz
    ├── 021909498fc2ae8c27f6a0acb20519d8f4e2f5e6.nq.gz
    ├── 021ad605f3feec1885a0fdf54416314a64c0447b.nq.gz
    ├── 021f7f9738a787f3e74a30ec482b0c133c2fa3e8.nq.gz
    ├── 022d8fa289a7de98bc4d122effc1336fd1c202cb.nq.gz
    ├── 022e70a7fd28543ddc6231479244dcee98a869ad.nq.gz
    ├── 023098b114ab7185710267d1e81bd666684bcc77.nq.gz
    ├── 0241ac5aef5aed156a3bd494863ada71433befe9.nq.gz
    ├── 02498249ef96f58070c9ca3a8a8da7e5b3749d9d.nq.gz
    ├── 024aff382347cf22c2e68558b4426b84f8298c5a.nq.gz
    ├── 024b9f26221696caaeab7e6a13b540ab0c2f191d.nq.gz
    ├── 0253371d3b9cc035babeb3616940899ed1199124.nq.gz
    ├── 02546a2b76859c301774bd832152e53fa33fe3ca.nq.gz
    ├── 0255af047dc040524c5a1525dba558878777d657.nq.gz
    ├── 025c492860266480443f55d581458d1ab30a39ce.nq.gz
    ├── 02636fb66b0ce33d824cc2a42ae5747c9ab26e86.nq.gz
    ├── 026a57699afd6ea05e9ef42dc2035454f8865715.nq.gz
    ├── 026fb29298d127247488d0550616094ceb42f7c9.nq.gz
    ├── 0270696b03ecb610ea19c2678efdb7a0cb059983.nq.gz
    ├── 02807a758890f831aeed763679a0fe4943600ca8.nq.gz
    ├── 0285cb5303c7129e2020e23e0e9dddc8e4bcb2d3.nq.gz
    ├── 02ab0a1f2be8ab2446ed518beac0b3ed954722c2.nq.gz
    ├── 02b95ad24525c6443bab4d280fa29d45cfac2c13.nq.gz
    ├── 02b9d24c84d9f60933b3f521933649079736c8be.nq.gz
    ├── 02c3a072713d57d5938a203e4a507c6be0216d07.nq.gz
    ├── 02ceb512f0c837c2416aee2f9af6cc5bb81a34d8.nq.gz
    ├── 02d168e02de1b5845bffed4502d964e43146079e.nq.gz
    ├── 02d3c88c4662f28700968ddae39f8ad4401c4bc9.nq.gz
    ├── 02d5daa101986b792b3ae1699a26024fb504e0fc.nq.gz
    ├── 02d733a503eeba81db8e9dbbe1ad4ad16b27ff1d.nq.gz
    ├── 02d737c9e8ad9c64f3d966f705afc556098d6e7c.nq.gz
    ├── 02d749e2e185d5a632b287f97fe00bf8095a2d15.nq.gz
    ├── 02db325046b0d783dd2c3140b97e0caf5340b3d8.nq.gz
    ├── 02e32dcb93186d9a38c0790d7eac14b649bd8020.nq.gz
    ├── 02e688d00b77d392fe5a24ec7cc9455b8a5f2f89.nq.gz
    ├── 02e9cfa70d79730d9f6530bfcdc668f81effb70f.nq.gz
    ├── 02f5e55734aa3382e891f99c448c59e21015c920.nq.gz
    ├── 02fbb6d059c7a7492374b8c7930256f72e0de6a6.nq.gz
    ├── 030045548604a9f98d6d818a55d6616e97820ce9.nq.gz
    ├── 030dd57aa092b3ec4b69335d3de27514fe0a244a.nq.gz
    ├── 031156dec53a79d4972bdad8beb3b4367fb7e3d3.nq.gz
    ├── 0311c871d41c64cd757cc3c7ea894b1768d98c34.nq.gz
    ├── 031fb4cdb61b7fd1ca3602f7a9683949d695715e.nq.gz
    ├── 03219ae78f2d3c26fbcecd27690ae6f3ece4640d.nq.gz
    ├── 0333da569a4ee7f2f8a1357cf40071e635b51101.nq.gz
    ├── 033f714ed1ce6bd568a63fb4fe23113261de36da.nq.gz
    ├── 034f782b832a5199a45049e21526972fe089d243.nq.gz
    ├── 034ff2b6dcc2e78bfdf272e7f8a0b3a4b2aa7f1d.nq.gz
    ├── 035012e3b284a32f5d290008d437aa8de068920e.nq.gz
    ├── 0351156e93922b486f1aea6a46e942ed7c566058.nq.gz
    ├── 035a8a404719c950f7cb9e2b96d081ef5b56bd6d.nq.gz
    ├── 035e5a93d2aea52b2b3b701fcf85a2a7e8217e6b.nq.gz
    ├── 0369cf81c193773ae5bb20b88cf54eeef745e9b2.nq.gz
    ├── 0375b7883ab03747084be010f203737807f35afe.nq.gz
    ├── 0379cea8cab93a930fe2497942db5c8a6b5a82db.nq.gz
    ├── 037e1f5ab1145950aa8e62eb64f4c97463a1bd66.nq.gz
    ├── 0383dc52f7be76be5893caf9f12e05e7c0aef7e6.nq.gz
    ├── 038501639ca3db6d777b0ae83b181d9f2e3c4f0c.nq.gz
    ├── 038bb5e638514b12a3d6ae32c4933460ba3457c1.nq.gz
    ├── 0393ecdca9b9459f0af862910b0b40756d1513b5.nq.gz
    ├── 0395d0f5b11b9df061342d396517b1f52d2e77f7.nq.gz
    ├── 0397ee292b4908e4fb657985ff250b7fa83135ef.nq.gz
    ├── 03a534572835ecee6464ff4026aa1f9a1ff3116a.nq.gz
    ├── 03b6d1fddd4ec90bdf3ffb4e51cc94d073e63ceb.nq.gz
    ├── 03bb1845866bf22888133d830940761b67c259de.nq.gz
    ├── 03bf2e2c3f09889b16f1fd61fc9fc9639ebe592c.nq.gz
    ├── 03c1f9a396e4318ee6e78daa355e994d0a1ab558.nq.gz
    ├── 03cdfa32438d36dffbb59a0f0841ffe97778e1ff.nq.gz
    ├── 03d1733c498dadd215b9b205009140085478bff3.nq.gz
    ├── 03d178f72d6ef3a2c4c5878b33efdf7cbc86d808.nq.gz
    ├── 03d3b2120c9861e90cf80dcb5d8fe0b3346c70cc.nq.gz
    ├── 03de7e68d7d1b9bdb40b88fec8fb07383936bafe.nq.gz
    ├── 03e393195fea716181fe0e49682a44fe9108356a.nq.gz
    ├── 03e95c4e010c546dd57da2d50d679a446548b76b.nq.gz
    ├── 03faee0e9ce455e08cd75c3a46d42e86c75f168a.nq.gz
    ├── 040b643a29fc182c7edd4ad245b0719b0ce6a72b.nq.gz
    ├── 041b15330821fed0bf4c7fc11dd41c42c7cee3e4.nq.gz
    ├── 042441bc9cc3a1022fbcb77ba9f2f6b44849c18d.nq.gz
    ├── 042d5e615bd3bcd83073b1948d597d3953fe236c.nq.gz
    ├── 0443cf2fdb257958c781d7a618dd9f3eed8b33db.nq.gz
    ├── 044a7da7f722492b6abf25ad9bd1b3eb713c1daf.nq.gz
    ├── 044f1f6ad66dc1312e4841b627eaa216f055c846.nq.gz
    ├── 045199efecb2a18018ddb4cacdb5ada758b918a5.nq.gz
    ├── 045ff99b05f6b195f0ffd06eeaadc854761c5f04.nq.gz
    ├── 04606860d7207a3ea7e39f5c06ed41879d9b7601.nq.gz
    ├── 046d8a0f01f21669674b362211e9ad3133e4724a.nq.gz
    ├── 047e4cb824b5f75f15191df22d9c1f6f53cca782.nq.gz
    ├── 0487a74597421b57ae88c4c4475cbb6cca7e3e53.nq.gz
    ├── 04a73e2f2fad74f7c4d161e4c726dbea9bf25d9a.nq.gz
    ├── 04b093075225e6fe8d4a59cb60ffeb32d149bce6.nq.gz
    ├── 04b1b59b1c06873b0964b45c6dea8f2b9f328595.nq.gz
    ├── 04b32de561ff7bbec019dcd1d3dd8a70bdbce1af.nq.gz
    ├── 04b98bc03d16401e3868fb6a3c4c948250e70027.nq.gz
    ├── 04bf6beed6ae9a55b1a79fd76fc3578aee1afe54.nq.gz
    ├── 04c2761416bdcc53c4623e94a58afa562cd60a43.nq.gz
    ├── 04ccc7ff48470ca31dc0abebabf03cc648c595c3.nq.gz
    ├── 04d18bf42981fae899308a6d8ce8bb01330ea5bb.nq.gz
    ├── 04d25e5137b4f2b3d870becb9686163950f14b70.nq.gz
    ├── 04d483e3bfcd1530f2cdb106bf899cf6db9b1028.nq.gz
    ├── 04efbdf48dea1d0b2072e369d7432815ff907966.nq.gz
    ├── 04f922e366f8d6c38de42cfe9c03ec5a96de74a5.nq.gz
    ├── 05027512e58cfa9cebce83d5bc389b171b55afed.nq.gz
    ├── 050cb44e450149943d6dd0f1dcaebef7c9df5570.nq.gz
    ├── 0510ee560834ba9001838a05d6ce2dde9da38521.nq.gz
    ├── 0511750ab37a22469e0309c067ecda76abd9f7a6.nq.gz
    ├── 0516a29570f1ca3f35c85480807b27b3990e9e0f.nq.gz
    ├── 0517a59d9acd248b0c83991a3dba762ae590d120.nq.gz
    ├── 052eb04895c4ba40afbfd7e84ccc17e66f17ad63.nq.gz
    ├── 053514cd7897ea738f4a7bcd66e2101de8bec7de.nq.gz
    ├── 053772380cc3493485fb657a11f7f63680852c71.nq.gz
    ├── 055de6d0bb5729b8cd505643b5cde0d4d4efda36.nq.gz
    ├── 056766f14a5f002db6d51b27070eed0703b77fb6.nq.gz
    ├── 0567c386d0186262856afd8731acd6e39973d6e6.nq.gz
    ├── 056aa39b7299dc3941d360452d5e780d30fa6ee0.nq.gz
    ├── 056b91d8a556ab20ca1e007ac84339498cceab35.nq.gz
    ├── 056d086665fa0f3caa7f0fedb24a7b1c865038cc.nq.gz
    ├── 0573e86947c113c7c72eaf33f95404ed76a304eb.nq.gz
    ├── 057a21d2981fc820c2e44ca698bb5fd1559e484b.nq.gz
    ├── 05874888ef5a17fe4ff455358cfa3b3883b55e55.nq.gz
    ├── 058ae039f55148ceb93e5d5b134915dfd27b5075.nq.gz
    ├── 058b2b267e5629bdb6d8105d1776714ebd91abf2.nq.gz
    └── 058bde675e1a029edd1141a68866646bea59594b.nq.gz

8 directories, 200 files
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

## Source repository

[apache/jena](https://github.com/apache/jena)

---
*Parsed on 2026-04-09 by [repolex](https://repolex.ai)*
