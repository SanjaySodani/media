* A simple multiselect dropdown which has **Select All** and **Search** options. 
* You can use a simple list or a list of maps.

## Features

https://user-images.githubusercontent.com/88200484/219946035-d5dc8d82-eb14-43d5-a56d-fe217b25764d.mov

* Use `MultiSelectDropdown` for list of maps.
* Use `MultiSelectDropdown.simpleList` for a simple list.

## Getting started

* Add the package in your flutter project.
* Import the package `import 'package:multi_select_dropdown/multi_select_dropdown.dart';`.

## Usage

```dart
class MultiSelectExample extends StatelessWidget {
  const MultiSelectExample({super.key});

  final List myList2 = const ['Dog', 'Cat', 'Mouse', 'Rabbit'];

  final List myList = const [
    {'id': 'dog', 'label': 'Dog'},
    {'id': 'cat', 'label': 'Cat'},
    {'id': 'mouse', 'label': 'Mouse'},
    {'id': 'rabbit', 'label': 'Rabbit'},
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Column(
        children: [
          MultiSelectDropdown(
            list: myList,
            initiallySelected: const [],
            onChange: (newList) {
              // your logic
            },
          ),
          const SizedBox(
            height: 50,
          ),
          MultiSelectDropdown.simpleList(
            list: myList2,
            initiallySelected: const [],
            onChange: (newList) {
              // your logic
            },
            includeSearch: true,
            includeSelectAll: true,
          ),
        ],
      ),
    );
  }
}
```

> I will keep adding more functionalities.
