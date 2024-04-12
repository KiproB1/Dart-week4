# Dart-week4
Object oriented programming
// Task 1: Object-Oriented Model with Classes and Inheritance
class Animal {
  void makeSound() {
    print('Animal makes a sound');
  }
}

class Dog extends Animal {
  @override
  void makeSound() {
    print('Dog barks');
  }
}

// Task 2: Class Implementing an Interface
abstract class Shape {
  void draw();
}

class Circle implements Shape {
  @override
  void draw() {
    print('Drawing a circle');
  }
}

// Task 3: Class Overriding an Inherited Method
class Parent {
  void greet() {
    print('Hello from Parent');
  }
}

class Child extends Parent {
  @override
  void greet() {
    print('Hello from Child');
  }
}

// Task 4: Instance Initialized with Data from a File
class Person {
  late String name;
  late int age;

  Person(this.name, this.age);

  @override
  String toString() {
    return 'Name: $name, Age: $age';
  }
}

// Task 5: Method Demonstrating the Use of a Loop
void printNumbers() {
  for (int i = 1; i <= 5; i++) {
    print(i);
  }
}

void main() {
  // Task 1
  Animal animal = Dog();
  animal.makeSound(); // Output: Dog barks

  // Task 2
  Circle circle = Circle();
  circle.draw(); // Output: Drawing a circle

  // Task 3
  Parent parent = Parent();
  parent.greet(); // Output: Hello from Parent

  Child child = Child();
  child.greet(); // Output: Hello from Child

  // Task 4
  var person = Person('Alice', 30);
  print(person); // Output: Name: Alice, Age: 30

  // Task 5
  printNumbers(); // Output: 1 2 3 4 5
}
