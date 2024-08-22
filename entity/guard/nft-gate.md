### NFT Gate

#### Props

- `requiredCollection`: Address of the collection
- `chain`: Chain to which the collection belongs

#### Spec

```TS
interface NftGate {
  requiredCollection: string;
  chain: string;
}
```

#### Example

```json
{
  "nftGate": {
    "requiredCollection": "0xbd3531da5cf5857e7cfaa92426877b022e612cf8",
    "chain": "ETH"
  }
}
```

multi chain

```json
{
  "nftGate": [
    {
      "requiredCollection": "0xbd3531da5cf5857e7cfaa92426877b022e612cf8",
      "chain": "ETH"
    },
    {
      "requiredCollection": "0xbd3531da5cf5857e7cfaa92426877b022e612cf8",
      "chain": "BNB"
    }
  ]
}
```
