### Guard

A modular piece of code that can restrict access

#### Example:

From this requirement

```
User can claim airdrop only if they hold a `pudgy pegiun` in ETH and each user only claim one time
```

```json
{
  "guards": {
    "claimLimit": {
      "limit": 1
    },
    "nftGate": {
      "requiredCollection": "0xbd3531da5cf5857e7cfaa92426877b022e612cf8",
      "chain": "ETH"
    }
  }
}
```

#### Guards

- [Claim limit](./claim-limit.md)

- [NFT gate](./nft-gate.md)

- [Token gate](./token-gate.md)

- [Allow list](./allow-list.md)
