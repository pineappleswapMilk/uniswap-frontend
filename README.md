# Uniswap Interface

[![Lint](https://github.com/Uniswap/uniswap-interface/workflows/Lint/badge.svg)](https://github.com/Uniswap/uniswap-interface/actions?query=workflow%3ALint)
[![Tests](https://github.com/Uniswap/uniswap-interface/workflows/Tests/badge.svg)](https://github.com/Uniswap/uniswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for PineappleSwap -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [PineappleSwap.io](https://PineappleSwap.io/)
- Interface: [app.PineappleSwap.io](https://app.PineappleSwap.io)
- Docs: [PineappleSwap.io/docs/](https://PineappleSwap.io/docs/)
- Twitter: [@PineappleSwapio](https://twitter.com/PineappleSwapio)
- Email: [PineappleSwap@mail.com](mailto:PineappleSwap@mail.com)
- Discord: [PineappleSwap]()
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Accessing the PineappleSwap Interface

To access the PineappleSwap Interface, use an IPFS gateway link from the
[latest release](https://github.com/PineappleSwap/PineappleSwap-interface/releases/latest), 
or visit [app.PineappleSwap.io](https://app.PineappleSwap.io).

## Listing a token

Please see the
[@PineappleSwap/default-token-list](https://github.com/PineappleSwap/default-token-list) 
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"` 

Note that the interface only works on testnets where both 
[PineappleSwap V2](https://PineappleSwap.io/docs/v2/smart-contracts/factory/) and 
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.** 
CI checks will run against all PRs.

## Accessing PineappleSwap Interface V1

The PineappleSwap Interface supports swapping against, and migrating or removing liquidity from PineappleSwap V1. However,
if you would like to use PineappleSwap V1, the PineappleSwap V1 interface for mainnet and testnets is accessible via IPFS gateways 
linked from the [v1.0.0 release](https://github.com/PineappleSwap/PineappleSwap-interface/releases/tag/v1.0.0).
