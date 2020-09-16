# BSCswap Interface

[![Tests](https://github.com/bscswap/bscswap-interface/workflows/Tests/badge.svg)](https://github.com/bscswap/bscswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for BSCswap -- a protocol for decentralized exchange of Binance Smart Chain BEP20 tokens.

- Website: [bscswap.com](https://bscswap.com/)
- Docs: [uniswap.org/docs/](https://uniswap.org/docs/)
- Twitter: [@BSCswapProtocol](https://twitter.com/BSCswapProtocol)
- Email: [hyunsiklee@bscswap.com](mailto:hyunsiklee@bscswap.com)
- Discord: [BSCswap](https://discord.gg/xjNuc56)

## Accessing the BSCswap Interface

To access the BSCswap Interface, visit [bscswap.com](https://bscswap.com) which is hosted directly on gh-pages branch.

## Listing a token

Please see the
[@bscswap/default-token-list](https://github.com/bscswap/default-token-list)
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

Note that the interface only works on BSC testnets where both
[BSCswap Factory & Router Contract](https://github.com/bscswap/contracts/tree/master/contracts) and
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.**
CI checks will run against all PRs.
