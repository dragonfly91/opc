# Part 2: Introduction to Flutter

## 1

```dart
Scaffold(
  appBar: AppBar(
    title: const Text('App Bar'),
  ),
  body: const Center(
    child: Text(
      'Body',
      style: TextStyle(
        fontSize: 32,
      ),
    ),
  ),
)
```

## 2

```dart
        ElevatedButton(
          onPressed: () {},
          child: const Text(
            'PRESS ME',
            style: TextStyle(fontSize: 24),
          ),
        )
```

## 3

```dart
      const Center(
        child: Icon(
          Icons.home,
          size: 64,
        ),
      )
```

## 4

```dart
        Padding(
          padding: EdgeInsets.all(16),
          child: TextField(
            decoration: InputDecoration(
              border: OutlineInputBorder(),
              labelText: 'Name',
            ),
          ),
        )
```

## 5

```dart
        Row(
          mainAxisAlignment: MainAxisAlignment.spaceEvenly,
          children: const [
            Icon(Icons.home, size: 64),
            Icon(Icons.back_hand, size: 64),
            Icon(Icons.face, size: 64),
          ],
        )
```

## 6

```dart
      const Padding(
        padding: EdgeInsets.all(0),
        child: Icon(
          Icons.list,
          size: 80,
        ),
      )
```

## 7

```dart
      Center(
        child: Row(
          children: const [
            Icon(Icons.add_a_photo, size: 42),
            Icon(Icons.add_a_photo, size: 42),
            Icon(Icons.add_a_photo, size: 42),
          ],
        ),
      )
```

```dart
SizedBox(width: 16)
```

## 8

```dart
        Text(
          'Hello',
          style: TextStyle(fontSize: 42),
        )
```

## 9

```dart
        Container(
          padding: const EdgeInsets.all(16.0),
          decoration: BoxDecoration(
            border: Border.all(color: Colors.blueAccent),
          ),
          child: const Text(
            'Hello',
            style: TextStyle(fontSize: 42),
          ),
        )
```
