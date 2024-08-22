### Token Gate

#### Props

- `address`: Address of the collection
- `chain`: Chain to which the collection belongs
- `amount` : minimum balance of user

#### Spec

```TS
interface TokenGate {
  address: string;
  chain: string;
  amount: number;
}
```

#### Example

```json
{
  "tokenGate": {
    "address": "0x4B4c8ABe2dC873F04068075908F4719554b2cb2C",
    "chain": "ETH",
    "amount": 300
  }
}
```

multi chain

```json
{
  "tokenGate": [
    {
      "address": "0x4B4c8ABe2dC873F04068075908F4719554b2cb2C",
      "chain": "ETH",
      "amount": 300
    },
    {
      "address": "0x4B4c8ABe2dC873F04068075908F4719554b2cb2C",
      "chain": "BNB",
      "amount": 100
    }
  ]
}
```
