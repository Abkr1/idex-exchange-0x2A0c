# IDEX Exchange — 0x2A0c0dBECc7E4D658f48E01e3fA353F44050c208

Extracted verified source for the **IDEX decentralized exchange** contract on **Ethereum mainnet**.

- **Address:** [`0x2A0c0dBECc7E4D658f48E01e3fA353F44050c208`](https://etherscan.io/address/0x2A0c0dBECc7E4D658f48E01e3fA353F44050c208)
- **Chain ID:** 1 (Ethereum mainnet)
- **Contract name:** `Exchange` (`src/Exchange.sol`, plus `Token` interface in the same file)
- **Compiler:** Solidity `0.4.16+commit.d7661dd9`, optimizer enabled (200 runs)
- **Verification:** verified on Etherscan; Sourcify reports `match` (partial — metadata hash differs, sources match)
- **Source of this repo:** Sourcify v2 API (`stdJsonInput` + `abi`); original Sourcify path was `Exchange.sol`, placed at `src/Exchange.sol` for a standard Foundry layout with no logic changes

This repo is a mirror for reading / auditing / reuse. It is **not** the upstream IDEX repo.

## Layout

```
idex-exchange-0x2A0c/
  src/
    Exchange.sol   # main contract + Token interface (pragma ^0.4.16)
  abi.json         # contract ABI from Sourcify (33 entries)
  foundry.toml     # solc 0.4.16, optimizer 200 runs
```

## Build

Requires [Foundry](https://book.getfoundry.sh/). The first build downloads solc 0.4.16 automatically.

```shell
forge build
```

## Test

No tests are vendored (the verified bundle contains only deployment sources). Add your own under `test/`:

```shell
forge test
```

## License

No SPDX identifier in the original source (pre-SPDX era contract). No new license grant is made by this mirror; check the upstream IDEX project for terms.
