## Parameters

| Parameter Name | Description |
| -------------- | ----------- |
| list | List of options to select from |
| label | `label` key in a Map to show as an option. Defaults to 'label' |
| id | `id` key in a Map to identify an item. Defaults to 'id' |
| onChange | `onChange` callback, passes new list as argument |
| numberOfItemsLabelToShow | Number of items to show as text, beyond that it will show `n` selected |
| initiallySelected | Initially selected list |
| boxDecoration | Decoration for anchor element |
| isLarge | Dropdown size |
| width | Anchor and modal width |
| whenEmpty | Text to show when nothing is selected |
| includeSelectAll | Includes a select all button when `true` |
| includeSearch | Includes a search option when `true` |
| textStyle | `TextStyle?` for the text on anchor element |
| duration | `Duration?` for debounce in search option. Defaults to 300 milliseconds. |
