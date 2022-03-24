# Choice JSON Format

This is the format of a JSON file describing a choice. They need to be placed inside the `choices` folder within your namespace.

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`powers` | [Array](../data_types/array/) of [Identifiers](../data_types/identifier/) | _optional_ | IDs of the powers this choice should have.
`icon` | [Item Stack](../data_types/item_stack/) | _optional_ | The item stack which is displayed as the icon for the description button for the choice
`name` | [String](../data_types/string/) | _optional_ | The display name of the choice.
`description` | [String](../data_types/string/) | _optional_ | The description of the choice.
`action_on_chosen` | [Action](https://origins.readthedocs.io/en/latest/types/entity_condition_types/) | _optional_ | The description of the choice.

### Example

```json
{
    "powers": [
        "example_pack:mana_bar",
        "example_pack:mana_recharge",
        "example_pack:mana_recharge_2"
    ],
    "icon": "minecraft:diamond",
    "name": "Magic User",
    "description": "You can harness mana to use in a staff!"
}
```
This example choice adds  with a `minecraft:diamond` as its icon.