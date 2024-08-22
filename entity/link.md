### Link

| Property    | Type                      | Description                                 | Example Value                       |
| ----------- | ------------------------- | ------------------------------------------- | ----------------------------------- |
| id          | String                    | Identifier for the link template            | 12345                               |
| title       | String                    | Title of the link                           | Motoko Airdrop                      |
| description | String                    | Brief summary of the action to be performed | This is motoko airdrop              |
| label       | String                    |                                             |                                     |
| icon        | String                    | Image for the link                          |                                     |
| guards      | [Guard](./guard/guard.md) | Guard for link                              | [example](./guard/guard.md#example) |
| layout      | [Layout](#layout)         | Layout for render the link                  | [example](#layout)                  |
| actions     | [Action](#action) Array   | Array of action                             | [example](#action-example)          |
| errors      | String                    |                                             |                                     |

### Action

| Property | Type                                      | Description                               | Example Value                             |
| -------- | ----------------------------------------- | ----------------------------------------- | ----------------------------------------- |
| href     | String                                    | Href to the action                        | /path/xyz                                 |
| label    | String                                    | Label for the the input                   | Claim                                     |
| params   | [Array ActionParameter](#actionparameter) | Query param for the link for input fields | [Array ActionParameter](#actionparameter) |

#### Action Example

```json
// for hard code value
{
  "label": "Buy 10 Sats",
  "href": "/buy?amount=10"
}

//for input value
{
  "label": "Buy",
  "href": "/buy?amount={amount}",
  "params": [
        {
            "name": "amount",
            "label": "Sats amount",
            "required": true
        }
    ]
}
```

### ActionParameter

| Property | Type    | Description          | Example Value |
| -------- | ------- | -------------------- | ------------- |
| name     | String  | Name of the action   | /path/xyz     |
| label    | String  | Label for the button | Claim         |
| required | boolean | Require of the param | true          |

### Layout

```TS
enum Layout {
    Left,
    Right,
    Central
}
```
