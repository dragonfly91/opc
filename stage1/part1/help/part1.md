# Part 1: Introduction to Dart

## 1

```dart
String s = 'hello';

print(s);
```

## 2

```dart
String firstName = 'Samuel';
String lastName = 'Bangari';
int age = 30;
String nationality = 'Indian';

print(firstName);
print(lastName);
print(age);
print(nationality);
```

## 3

```dart
class Person {
  String firstName;
  String lastName;
  int age;
  String nationality;

  Person(
    this.firstName,
    this.lastName,
    this.age,
    this.nationality,
  );
}
```

## 4

```dart
Person p = Person(
  'Samuel', 
  'Bangari', 
  30, 
  'Indian',
);

print(p.firstName);
print(p.lastName);
print(p.age);
print(p.nationality);
```

## 5

```dart
List<String> l = [];

l.add('Hello');
l.add('my');
l.add('name');
l.add('is');
l.add('Samuel');

print(l);

l.remove('Hello');

print(l);
```

## 6

```dart
List<Person> l = [];

l.add(Person('Samuel', 'Bangari', 31, 'Indian'));
l.add(Person('Mami', 'Shimano', 23, 'Japanese'));

print(l.length);

print(l[0].firstName);
print(l[1].firstName);

l.removeAt(0);

print(l.length);

print(l[0].firstName);
```

## 7

```dart
for (var i = 0; i < 10; i++) {
  print(i);
}
```

## 8

```dart
List<int> l = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55];

for (var item in l) {
  print(item);
}
```