### Allow list

#### Props

- `addresses`: Addresses of user
- `chain`: Chain to which the collection belongs

#### Spec

```TS
interface AllowList {
  chain: string;
  addresses: string[];
}
```

#### Example

```json
{
  "allowList": {
    "chain": "ETH",
    "addresses": [
      "0xbd3531da5cf5857e7cfaa92426877b022e612cf8"
      //.. other address
    ]
  }
}
```

multi chain

```json
{
  "allowList": [
    {
      "chain": "ETH",
      "addresses": [
        "0xbd3531da5cf5857e7cfaa92426877b022e612cf8"
        //.. other address
      ]
    },
    {
      "chain": "SOL",
      "addresses": [
        "3caZyGZLLveCt1if6GUV2n3TTotfFQhAEVkn31rGSouC"
        //.. other address
      ]
    }
  ]
}
```
