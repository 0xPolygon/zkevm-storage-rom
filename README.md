> [!WARNING]
> **This repository is deprecated and no longer maintained.**
>
> Polygon zkEVM has been retired. Polygon CDK chains now run on
> [cdk-op-reth](https://github.com/0xPolygon/cdk-op-reth) and settle to the
> [Agglayer](https://github.com/agglayer/agglayer) with pessimistic proofs and
> full execution proofs. This code is kept for reference only. It will not
> receive bug fixes, security patches, or releases.
>
> **Use instead:**
> - Proving: [agglayer/provers](https://github.com/agglayer/provers)
> - Agglayer node: [agglayer/agglayer](https://github.com/agglayer/agglayer)
> - Docs: [docs.polygon.technology](https://docs.polygon.technology)
>
> **Have funds locked in contracts on zkEVM mainnet?** See
> [zkevm-proof-of-ownership-kit](https://github.com/agglayer/zkevm-proof-of-ownership-kit).
>
> Security issues in live Polygon systems: see [SECURITY.md](https://github.com/0xPolygon/.github/blob/main/SECURITY.md).

# zkASM Storage Compiler
This repo compiles .zkasm storage to a json file

## Setup
```
npm install
npm run build
```
## Usage
Generate json file from zkasm storage file:
```sh
node src/zkasmstorage.js <inputFile.zkasm> -o <outFile.json>
```
Example:
```sh
node src/zkasmstorage.js zkasm/storage_sm.zkasm -o build/storage_sm_rom.json
```
or
```sh
npm run build:rom
```
