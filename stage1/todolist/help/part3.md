# Part 3: TODOLIST App

## 1

```dart
class _MyHomePageState extends State<MyHomePage> {
  List<String> todoItems = [
    'Do dishes',
    'Do laundry',
    'Buy milk',
  ];
}
```

## 2

```dart
  @override
  Widget build(BuildContext context) {
    List<Widget> todoItemWidgets = [];

    for (var todoItem in todoItems) {
      todoItemWidgets.add(_buildTodoItem(todoItem));
    }

    return Scaffold(
      appBar: AppBar(
        title: const Text('TODOLIST'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16),
        child: Column(
          children: [
            _buildInputBox(),
            const SizedBox(height: 16),
            Column(
              children: todoItemWidgets,
            ),
          ],
        ),
      ),
    );
  }
```

## 3

```dart
  Widget _buildInputBox() {
    return Row(
      children: const [
        Expanded(
          child: TextField(
            decoration: InputDecoration(
              border: OutlineInputBorder(),
              hintText: 'Add a new todo item',
            ),
          ),
        ),
        SizedBox(width: 16),
        Icon(Icons.send_outlined),
      ],
    );
  }
```

## 4

```dart
  Widget _buildTodoItem(String todoItem) {
    return Padding(
      padding: const EdgeInsets.symmetric(vertical: 4),
      child: Row(
        mainAxisAlignment: MainAxisAlignment.spaceBetween,
        children: [
          Row(
            children: [
              const Icon(Icons.check_box_outline_blank),
              const SizedBox(width: 8),
              Text(todoItem),
            ],
          ),
          const Icon(Icons.delete),
        ],
      ),
    );
  }
```

## 5

```dart
        IconButton(
          onPressed: () {},
          icon: const Icon(Icons.send_outlined),
        )
```

## 6

```dart
TextEditingController controller = TextEditingController();
```

## 7

```dart
controller: controller,
```

## 8

```dart
            setState(() {
              todoItems.add(controller.text);
            });
```

## 9

```dart
controller.clear();
```

## 10

```dart
class TodoItem {
  String content;
  bool checked;
  TodoItem(this.content, this.checked);
}
```

## 11

```dart
TodoItem(controller.text, true)
```

## 12

```dart
              IconButton(
                onPressed: () {},
                icon: const Icon(Icons.check_box_outline_blank),
              )
```

## 13

```dart
todoItem.checked ? Icons.check_box_outlined : Icons.check_box_outline_blank
```

## 14

```dart
                  setState(() {
                    todoItem.checked = !todoItem.checked;
                  });
```

## 15

```dart
          IconButton(
            onPressed: () {},
            icon: const Icon(Icons.delete),
          )
```

## 16

```dart
              setState(() {
                todoItems.removeWhere((element) => element.content == todoItem.content);
              });
```