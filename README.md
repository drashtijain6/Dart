# Dart
1.void main() {
  print("Hello, Dart! Welcome to Programming.");
}


2.void main() {
  
  int a = 10;
  int b = 5;

  int sum = a + b;
  int difference = a - b;
  int product = a * b;
  double quotient = a / b;

  print("Sum: $sum");
  print("Difference: $difference");
  print("Product: $product");
  print("Quotient: $quotient");
}


3.void main() {
 
  int num = 11;

  if (num % 2 == 0) {
    print("The number is Even.");
  } else {
    print("The number is Odd.");
  }
}


4.int add(int a, int b) {
  return a + b;
}

int subtract(int a, int b) {
  return a - b;
}

int multiply(int a, int b) {
  return a * b;
}

double divide(int a, int b) {
  return a / b;
}

void main() {
 
  int a = 8;
  int b = 4;

  print("Addition: ${add(a, b)}");
  print("Subtraction: ${subtract(a, b)}");
  print("Multiplication: ${multiply(a, b)}");
  print("Division: ${divide(a, b)}");
}


5.void main() {
  int n = 10; 
  int t1 = 0, t2 = 1;

  print("Fibonacci Series:");
  for (int i = 0; i < n; i++) {
    print(first);
    int next = t1 + t2;
    t1 = t2;
    t2 = next;
  }
}


6.void main() {
  
  List<int> numbers = [5, 3, 8, 1, 2];
  numbers.add(7);

  numbers.sort();
  print("Sorted List: $numbers");
}


7.void main() {
  
  Set<int> numbers = {1, 2, 3, 4};
  numbers.add(5);
  numbers.remove(2);

  print("Final Set: $numbers");
}


8.void main() {

  Map<String> person = {
    'name': 'Alice',
    'age': 25,
    'city': 'New York'
  };

  person['country'] = 'USA';
  person['age'] = 26;

  print("Updated Map: $person");
}


9.void main() {
  List<int> numbers = [5, 2, 9, 1, 5, 6];

  for (int i = 0; i < numbers.length - 1; i++) {
   for (int j = 0; j < numbers.length - i - 1; j++) {
      if (numbers[j] > numbers[j + 1]) {
        
        int temp = numbers[j];
        numbers[j] = numbers[j + 1];
        numbers[j + 1] = temp;
      }
    }
  }

  print("Sorted List: $numbers");
}


11.class Car {

  String brand;
  String model;
  int year;

  Car(this.brand, this.model, this.year);

  void displayInfo() {
    print("Car Details:");
    print("Brand: $brand");
    print("Model: $model");
    print("Year: $year");
  }
}

void main() {
  Car car = Car('Toyota', 'Corolla', 2020);
  car.displayInfo();
}



12.class Animal {
 
  void makeSound() {
    print("Animal makes a sound");
  }
}

class Dog extends Animal {
  
  void makeSound() {
    print("Dog barks");
  }
}

void main() {
 
  Animal animal = Animal();
  animal.makeSound(); 

  Dog dog = Dog();
  dog.makeSound();
}


13.void greet(String name,[String message= "Welcome"])
 {
  print("Hello $name, $message");
}

void main()
{
  greet("Alice");        
  greet("Bob", "Good Morning");
}


14.void main() {
  
  List<int> numbers = [1, 2, 3, 4, 5];

  numbers.forEach((number) {
    print("Square of $number: ${number * number}");
  });
}
