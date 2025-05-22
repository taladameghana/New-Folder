# New-Folder
1.Module 3-Core java
**Solution 1:
public class HelloWorld
{
    public static void main(String[] args)
    {
        System.out.println("Hello, World!");
    }
}
**Solution 2:
import java.util.Scanner;
public class Calculator {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        System.out.println("Enter two numbers:");
        int a = s.nextInt();
        int b = s.nextInt();
        s.nextLine(); 
        System.out.println("Choose an arithmetic operation: Addition, Subtraction, Multiplication, Division");
        String operation = s.nextLine();
        switch (operation) {
            case "Addition":
                System.out.println("Addition of two numbers is: " + (a + b));
                break;
            case "Subtraction":
                System.out.println("Subtraction of two numbers is: " + (a - b));
                break;
            case "Multiplication":
                System.out.println("Multiplication of two numbers is: " + (a * b));
                break;
            case "Division":
                if (b != 0) {
                    System.out.println("Division of two numbers is: " + ((double) a / b));
                } else {
                    System.out.println("Error! Division by zero.");
                }
                break;
            default:
                System.out.println("Invalid operation selected.");
        }
    }
}
**Solution 3:
import java.util.Scanner;
public class EvenOddChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int number = scanner.nextInt();
        if (number % 2 == 0) {
            System.out.println(number + " is even.");
        } else {
            System.out.println(number + " is odd.");
        }
    }
}
**Solution 4:
import java.util.Scanner;
public class LeapYearChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);\
        System.out.print("Enter a year: ");
        int year = scanner.nextInt();
        if (year % 4 == 0) {
            if (year % 100 == 0) {
                if (year % 400 == 0) {
                    System.out.println(year + " is a leap year.");
                } 
                else 
                {
                    System.out.println(year + " is not a leap year.");
                }
            } 
            else 
            {
                System.out.println(year + " is a leap year.");
            }
        } 
        else
        {
            System.out.println(year + " is not a leap year.");
        }
    }
}
**Solution 5:
import java.util.Scanner;
public class MultiplicationTable {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();
        for (int i = 1; i <= 10; i++) {
            int result = number * i;
            System.out.println(number + " x " + i + " = " + result);
        }
    }
}
**Solution 6:
public class DataTypeDemo {
    public static void main(String[] args) {
        int myInt = 25;
        float myFloat = 3.14f;
        double myDouble = 123.456;
        char myChar = 'A';
        boolean myBoolean = true;
        System.out.println("Integer value: " + myInt);
        System.out.println("Float value: " + myFloat);
        System.out.println("Double value: " + myDouble);
        System.out.println("Character value: " + myChar);
        System.out.println("Boolean value: " + myBoolean);
    }
}
**Solution 7:
public class TypeCastingExample {
    public static void main(String[] args) {
        double myDouble = 9.78;
        int myInt = (int) myDouble;
        System.out.println("Original double value: " + myDouble);
        System.out.println("After casting to int: " + myInt);
        int anotherInt = 42;
        double anotherDouble = anotherInt;
        System.out.println("Original int value: " + anotherInt);
        System.out.println("After casting to double: " + anotherDouble);
    }
}
**Solution 8:
public class OperatorPrecedenceDemo {
    public static void main(String[] args) {
        int result1 = 10 + 5 * 2;
        int result2 = (10 + 5) * 2;
        int result3 = 100 / 10 + 5;
        int result4 = 100 / (10 + 5);
        int result5 = 2 + 3 * 4 - 5;
        int result6 = 2 + (3 * (4 - 5));
        System.out.println("Result 1 (10 + 5 * 2): " + result1);
        System.out.println("Result 2 ((10 + 5) * 2): " + result2);
        System.out.println("Result 3 (100 / 10 + 5): " + result3);
        System.out.println("Result 4 (100 / (10 + 5)): " + result4);
        System.out.println("Result 5 (2 + 3 * 4 - 5): " + result5);
        System.out.println("Result 6 (2 + (3 * (4 - 5))): " + result6);
    }
}
**Solution 9:
import java.util.Scanner;
public class GradeCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter marks out of 100: ");
        int marks = scanner.nextInt();
        if (marks < 0 || marks > 100) {
            System.out.println("Invalid input. Please enter marks between 0 and 100.");
        } else {
            char grade;
            if (marks >= 90) {
                grade = 'A';
            } else if (marks >= 80) {
                grade = 'B';
            } else if (marks >= 70) {
                grade = 'C';
            } else if (marks >= 60) {
                grade = 'D';
            } else {
                grade = 'F';
            }
            System.out.println("Grade: " + grade);
        }
    }
}
**Solution 10:
import java.util.Scanner;
public class NumberGuessingGame {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int targetNumber = 1 + (int) (100 * Math.random());
        int userGuess = 0;
        int attempts = 0;
        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I have selected a number between 1 and 100.");
        System.out.println("Try to guess it!");
        while (userGuess != targetNumber) {
            System.out.print("Enter your guess: ");
            userGuess = scanner.nextInt();
            attempts++;
            if (userGuess < targetNumber) {
                System.out.println("The number is higher than " + userGuess + ". Try again.");
            } else if (userGuess > targetNumber) {
                System.out.println("The number is lower than " + userGuess + ". Try again.");
            } else {
                System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
            }
        }
    }
}
**Solution 11:
import java.util.Scanner;
public class FactorialCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a non-negative integer: ");
        int number = scanner.nextInt();
        if (number < 0) {
            System.out.println("Factorial is not defined for negative numbers.");
        } else {
            long factorial = 1;
            for (int i = 1; i <= number; i++) {
                factorial *= i;
            }
            System.out.println("Factorial of " + number + " is: " + factorial);
        }
    }
}
**Solution 12:
public class Calculator {
    public int add(int a, int b) {
        return a + b;
    }
    public double add(double a, double b) {
        return a + b;
    }
    public int add(int a, int b, int c) {
        return a + b + c;
    }

    public static void main(String[] args) {
        Calculator calc = new Calculator();
        System.out.println("Sum of a and b (int): " + calc.add(5, 10));
        System.out.println("Sum of a and b (double): " + calc.add(5.5, 10.5));
        System.out.println("Sum of a, b, and c (int): " + calc.add(5, 10, 15));
    }
}
**Solution 13:
import java.util.Scanner;
public class Fibonacci {
    // Recursive method to calculate the nth Fibonacci number
    public static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        }
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a positive integer n: ");
        int n = scanner.nextInt();
        if (n < 0) {
            System.out.println("Please enter a positive integer.");
        } else {
            System.out.println("The " + n + "th Fibonacci number is: " + fibonacci(n));
        }
    }
}
**Solution 14:
import java.util.Scanner;
public class ArraySumAverage {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of elements: ");
        int n = scanner.nextInt();
        int[] numbers = new int[n];
        System.out.println("Enter the elements:");
        int sum = 0;
        for (int i = 0; i < n; i++) {
            numbers[i] = scanner.nextInt();
            sum += numbers[i]; 
        }
        double average = (double) sum / n;
        System.out.println("Sum: " + sum);
        System.out.println("Average: " + average);
    }
}
**Solution 15:
import java.util.Scanner;
public class StringReversal {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String input = scanner.nextLine();
        StringBuilder reversed = new StringBuilder();
        for (int i = input.length() - 1; i >= 0; i--) {
            reversed.append(input.charAt(i));
        }
        System.out.println("Reversed string: " + reversed.toString());
    }
}
**Solution 16:
import java.util.Scanner;
public class PalindromeChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String input = scanner.nextLine();
        String cleanedInput = input.replaceAll("[^a-zA-Z0-9]", "").toLowerCase();
        if (isPalindrome(cleanedInput)) {
            System.out.println("\"" + input + "\" is a palindrome.");
        } else {
            System.out.println("\"" + input + "\" is not a palindrome.");
        }
    }
    private static boolean isPalindrome(String str) {
        int left = 0;
        int right = str.length() - 1;
        while (left < right) {
            if (str.charAt(left) != str.charAt(right)) {
                return false;
            }
            left++;
            right--;
        }
        return true;
    }
}
**Solution 17:
class Car {
    String make;
    String model;
    int year;
    public Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }
    public void displayDetails() {
        System.out.println("Car Details:");
        System.out.println("Make: " + make);
        System.out.println("Model: " + model);
        System.out.println("Year: " + year);
    }
}
public class Main {
    public static void main(String[] args) {
        Car car1 = new Car("Toyota", "Corolla", 2020);
        Car car2 = new Car("Honda", "Civic", 2022);
        car1.displayDetails();
        car2.displayDetails();
    }
}
**Solution 18:
    public void makeSound() {
        System.out.println("The animal makes a sound.");
    }
}
class Dog extends Animal {
    public void makeSound() {
        System.out.println("Bark");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.makeSound(); 
        Dog dog = new Dog();
        dog.makeSound(); 
        Animal myDog = new Dog();
        myDog.makeSound(); 
    }
}
**Solution 19:
interface Playable {
    void play();
}
class Guitar implements Playable {
    public void play() {
        System.out.println("Strumming the guitar: 'Strum strum strum!'");
    }
}
class Piano implements Playable {
    public void play() {
        System.out.println("Playing the piano: 'Ding dong ding!'");
    }
}
public class Main {
    public static void main(String[] args) {
        Playable guitar = new Guitar();
        Playable piano = new Piano();
        guitar.play();
        piano.play();
    }
}
**Solution 20:
import java.util.Scanner;
public class DivisionByZeroExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the numerator: ");
        int numerator = scanner.nextInt();
        System.out.print("Enter the denominator: ");
        int denominator = scanner.nextInt();
        try {
            int result = numerator / denominator;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Error: Cannot divide by zero.");
        } finally {
            scanner.close();
        }
    }
}
**Solution 21:
import java.util.Scanner;
class InvalidAgeException extends Exception {
    public InvalidAgeException(String message) {
        super(message);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        try {
            // Step 2: Validate the age
            if (age < 18) {
                throw new InvalidAgeException("Age must be 18 or above.");
            } else {
                System.out.println("Age is valid.");
            }
        } catch (InvalidAgeException e) {
            System.out.println("Caught Exception: " + e.getMessage());
        } finally {
            scanner.close();
        }
    }
}
**Solution 22:
import java.io.FileWriter;
import java.io.IOException;
import java.io.PrintWriter;
import java.util.Scanner;
public class FileWritingExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String userInput = scanner.nextLine();
        try (PrintWriter writer = new PrintWriter(new FileWriter("output.txt"))) {
            writer.println(userInput);
            System.out.println("Data has been written to output.txt.");
        } catch (IOException e) {
            System.out.println("An error occurred while writing to the file.");
            e.printStackTrace();
        } finally {
            scanner.close();
        }
    }
}
**Solution 23:
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;
public class FileReadingExample {
    public static void main(String[] args) {
        String filePath = "output.txt"; // Specify the path to your file
        try (BufferedReader reader = new BufferedReader(new FileReader(filePath))) {
            String line;
            while ((line = reader.readLine()) != null) {
                System.out.println(line); // Display each line
            }
        } catch (IOException e) {
            System.err.println("An error occurred while reading the file: " + e.getMessage());
        }
    }
}
**Solution 24:
import java.util.ArrayList;
import java.util.Scanner;
public class StudentNames {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<String> students = new ArrayList<>();
        System.out.println("Enter student names. Type 'done' to finish.");
        while (true) {
            System.out.print("Enter a name: ");
            String name = scanner.nextLine();
            if (name.equalsIgnoreCase("done")) {
                break;
            }

            students.add(name);
        }

        System.out.println("\nList of student names entered:");
        for (String student : students) {
            System.out.println(student);
        }
    }
}
**SOlution 25:
import java.util.HashMap;
import java.util.Scanner;
public class StudentIDNameMap {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        HashMap<Integer, String> studentMap = new HashMap<>();
        while (true) {
            System.out.println("\nMenu:");
            System.out.println("1. Add Student");
            System.out.println("2. Retrieve Student Name by ID");
            System.out.println("3. Display All Students");
            System.out.println("4. Exit");
            System.out.print("Choose an option: ");
            int choice = scanner.nextInt();
            scanner.nextLine();  // Consume newline
            switch (choice) {
                case 1:
                    System.out.print("Enter Student ID: ");
                    int id = scanner.nextInt();
                    scanner.nextLine();  // Consume newline
                    System.out.print("Enter Student Name: ");
                    String name = scanner.nextLine();
                    studentMap.put(id, name);
                    System.out.println("Student added successfully.");
                    break;
                case 2:
                    System.out.print("Enter Student ID to retrieve name: ");
                    int searchId = scanner.nextInt();
                    String studentName = studentMap.get(searchId);
                    if (studentName != null) {
                        System.out.println("Student Name: " + studentName);
                    } else {
                        System.out.println("No student found with ID: " + searchId);
                    }
                    break;

                case 3:
                    if (studentMap.isEmpty()) {
                        System.out.println("No students in the system.");
                    } else {
                        System.out.println("All Students:");
                        for (Integer studentId : studentMap.keySet()) {
                            System.out.println("ID: " + studentId + ", Name: " + studentMap.get(studentId));
                        }
                    }
                    break;

                case 4:
                    System.out.println("Exiting the program.");
                    scanner.close();
                    return;

                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }
}
**Solution 26:
public class ThreadExample {
    public static void main(String[] args) {
        Thread thread1 = new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 0; i < 5; i++) {
                    System.out.println("Thread 1: Message " + (i + 1));
                    try {
                        Thread.sleep(500); // Sleep for 500 milliseconds
                    } catch (InterruptedException e) {
                        System.out.println(e);
                    }
                }
            }
        });

        Thread thread2 = new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 0; i < 5; i++) {
                    System.out.println("Thread 2: Message " + (i + 1));
                    try {
                        Thread.sleep(500); // Sleep for 500 milliseconds
                    } catch (InterruptedException e) {
                        System.out.println(e);
                    }
                }
            }
        });

        // Start both threads
        thread1.start();
        thread2.start();
    }
}
**Solution 27:
import java.util.Arrays;
import java.util.List;
public class LambdaSortExample {
    public static void main(String[] args) {
        List<String> fruits = Arrays.asList("Banana", "Apple", "Mango", "Pineapple", "Grapes");
        System.out.println("Original List:");
        fruits.forEach(fruit -> System.out.println(fruit));
        fruits.sort((fruit1, fruit2) -> fruit1.compareTo(fruit2));
        System.out.println("\nSorted List:");
        fruits.forEach(fruit -> System.out.println(fruit));
    }
}
**Solution 28:
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;
public class EvenNumberFilter {
    public static void main(String[] args) {
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);
        List<Integer> evenNumbers = numbers.stream()
                                           .filter(n -> n % 2 == 0)
                                           .collect(Collectors.toList());
        System.out.println("Even numbers: " + evenNumbers);
    }
}
**Solution 29:
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;
public class PersonExample {
    public record Person(String name, int age) {}
    public static void main(String[] args) {
        Person alice = new Person("Alice", 30);
        Person bob = new Person("Bob", 25);
        Person charlie = new Person("Charlie", 35);
        List<Person> people = Arrays.asList(alice, bob, charlie);
        System.out.println("All Persons:");
        people.forEach(person -> System.out.println(person));
        List<Person> filteredPeople = people.stream()
                                             .filter(p -> p.age() >= 30)
                                             .collect(Collectors.toList());
        System.out.println("\nPersons aged 30 and above:");
        filteredPeople.forEach(person -> System.out.println(person));
    }
}
**Soloution 30:
public class TypeChecker {
    public static void main(String[] args) {
        System.out.println(checkType("Hello"));
        System.out.println(checkType(42));
        System.out.println(checkType(3.14));
        System.out.println(checkType(true));
        System.out.println(checkType(null));
    }
    public static String checkType(Object obj) {
        return switch (obj) {
            case String s -> "It's a String: " + s;
            case Integer i -> "It's an Integer: " + i;
            case Double d -> "It's a Double: " + d;
            case Boolean b -> "It's a Boolean: " + b;
            case null -> "It's null";
            default -> "Unknown type: " + obj.getClass().getName();
        };
    }
}
**Solution 31:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    age INT
);

INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;

public class JdbcExample {
    public static void main(String[] args) {
        String url = "jdbc:mysql:
        String user = "root";
        String password = "your_password";
        String query = "SELECT id, name, age FROM students";

        try (
            Connection conn = DriverManager.getConnection(url, user, password);
            Statement stmt = conn.createStatement();
            // Execute query and get result set
            ResultSet rs = stmt.executeQuery(query)
        ) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
**Solution 32:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

-- Sample data
INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;
public class StudentDAO {
    private static final String URL = "jdbc:mysql://localhost:3306/school";
    private static final String USER = "root";
    private static final String PASSWORD = "your_password"; // Replace with your MySQL password

    // Method to insert a new student
    public void insertStudent(String name, int age) {
        String query = "INSERT INTO students (name, age) VALUES (?, ?)";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            int rowsAffected = stmt.executeUpdate();
            System.out.println("Inserted " + rowsAffected + " row(s).");
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to update an existing student's details
    public void updateStudent(int id, String name, int age) {
        String query = "UPDATE students SET name = ?, age = ? WHERE id = ?";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            stmt.setInt(3, id);
            int rowsAffected = stmt.executeUpdate();
            if (rowsAffected > 0) {
                System.out.println("Updated student with ID " + id);
            } else {
                System.out.println("No student found with ID " + id);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to display all students
    public void displayStudents() {
        String query = "SELECT id, name, age FROM students";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             Statement stmt = conn.createStatement();
             ResultSet rs = stmt.executeQuery(query)) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
**Solution 33:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

-- Sample data
INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;

public class StudentDAO {
    private static final String URL = "jdbc:mysql://localhost:3306/school";
    private static final String USER = "root";
    private static final String PASSWORD = "your_password"; // Replace with your MySQL password

    // Method to insert a new student
    public void insertStudent(String name, int age) {
        String query = "INSERT INTO students (name, age) VALUES (?, ?)";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            int rowsAffected = stmt.executeUpdate();
            System.out.println("Inserted " + rowsAffected + " row(s).");
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to update an existing student's details
    public void updateStudent(int id, String name, int age) {
        String query = "UPDATE students SET name = ?, age = ? WHERE id = ?";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            stmt.setInt(3, id);
            int rowsAffected = stmt.executeUpdate();
            if (rowsAffected > 0) {
                System.out.println("Updated student with ID " + id);
            } else {
                System.out.println("No student found with ID " + id);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to display all students
    public void displayStudents() {
        String query = "SELECT id, name, age FROM students";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             Statement stmt = conn.createStatement();
             ResultSet rs = stmt.executeQuery(query)) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
public class Main {
    public static void main(String[] args) {
        StudentDAO dao = new StudentDAO();

        // Insert a new student
        dao.insertStudent("David", 24);

        // Update an existing student's details
        dao.updateStudent(1, "Alice Johnson", 21);

        // Display all students
        dao.displayStudents();
    }
}
**Solution 34:
project-root/
├── src/
│   ├── com.utils/
│   │   ├── module-info.java
│   │   └── com/utils/Utils.java
│   └── com.greetings/
│       ├── module-info.java
│       └── com/greetings/Greeting.java
└── out/
module com.utils {
    exports com.utils;
}
package com.utils;

public class Utils {
    public static String getGreeting() {
        return "Hello from Utils!";
    }
}
module com.greetings {
    requires com.utils;
}
package com.greetings;

import com.utils.Utils;

public class Greeting {
    public static void main(String[] args) {
        System.out.println(Utils.getGreeting());
    }
}
javac -d out/com.utils src/com.utils/module-info.java src/com/utils/Utils.java
javac -d out/com.greetings --module-path out -d out/com.greetings src/com.greetings/module-info.java src/com/greetings/Greeting.java
java --module-path out -m com.greetings/com.greetings.Greeting
**Solution 35:
import java.io.*;
import java.net.*;
import java.util.*;

public class ChatServer {
    private static final int PORT = 12345;
    private static Set<PrintWriter> clientWriters = new HashSet<>();

    public static void main(String[] args) throws IOException {
        System.out.println("Chat server started...");
        try (ServerSocket serverSocket = new ServerSocket(PORT)) {
            while (true) {
                new ClientHandler(serverSocket.accept()).start();
            }
        }
    }

    private static class ClientHandler extends Thread {
        private Socket socket;
        private PrintWriter out;
        private BufferedReader in;

        public ClientHandler(Socket socket) {
            this.socket = socket;
        }

        public void run() {
            try {
                in = new BufferedReader(new InputStreamReader(socket.getInputStream()));
                out = new PrintWriter(socket.getOutputStream(), true);
                synchronized (clientWriters) {
                    clientWriters.add(out);
                }
                String message;
                while ((message = in.readLine()) != null) {
                    System.out.println("Received: " + message);
                    synchronized (clientWriters) {
                        for (PrintWriter writer : clientWriters) {
                            writer.println(message);
                        }
                    }
                }
            } catch (IOException e) {
                System.out.println("Error handling client: " + e.getMessage());
            } finally {
                try {
                    socket.close();
                } catch (IOException e) {
                    System.out.println("Error closing socket: " + e.getMessage());
                }
                synchronized (clientWriters) {
                    clientWriters.remove(out);
                }
            }
        }
    }
}
import java.io.*;
import java.net.*;

public class ChatClient {
    private static final String SERVER_ADDRESS = "localhost";
    private static final int SERVER_PORT = 12345;

    public static void main(String[] args) throws IOException {
        try (Socket socket = new Socket(SERVER_ADDRESS, SERVER_PORT);
             BufferedReader in = new BufferedReader(new InputStreamReader(socket.getInputStream()));
             PrintWriter out = new PrintWriter(socket.getOutputStream(), true);
             BufferedReader userInput = new BufferedReader(new InputStreamReader(System.in))) {

            System.out.println("Connected to the chat server.");
            new ReadThread(in).start();

            String message;
            while ((message = userInput.readLine()) != null) {
                out.println(message);
            }
        }
    }

    private static class ReadThread extends Thread {
        private BufferedReader in;

        public ReadThread(BufferedReader in) {
            this.in = in;
        }

        public void run() {
            String message;
            try {
                while ((message = in.readLine()) != null) {
                    System.out.println(message);
                }
            } catch (IOException e) {
                System.out.println("Error reading from server: " + e.getMessage());
            }
        }
    }
}
**Solution 36:
<dependencies>
    <!-- Jackson for JSON parsing -->
    <dependency>
        <groupId>com.fasterxml.jackson.core</groupId>
        <artifactId>jackson-databind</artifactId>
        <version>2.13.1</version>
    </dependency>
    <!-- Gson for JSON parsing -->
    <dependency>
        <groupId>com.google.code.gson</groupId>
        <artifactId>gson</artifactId>
        <version>2.8.8</version>
    </dependency>
</dependencies>
import java.net.URI;
import java.net.http.HttpClient;
import java.net.http.HttpRequest;
import java.net.http.HttpResponse;
import java.io.IOException;

public class GitHubApiClient {
    public static void main(String[] args) throws IOException, InterruptedException {
        String user = "octocat"; // Replace with any GitHub username
        String url = "https://api.github.com/users/" + user;

        HttpClient client = HttpClient.newHttpClient();
        HttpRequest request = HttpRequest.newBuilder()
                .uri(URI.create(url))
                .header("Accept", "application/vnd.github.v3+json")
                .build();

        HttpResponse<String> response = client.send(request, HttpResponse.BodyHandlers.ofString());

        System.out.println("Status Code: " + response.statusCode());
        System.out.println("Response Body: " + response.body());
    }
}
import com.fasterxml.jackson.databind.JsonNode;
import com.fasterxml.jackson.databind.ObjectMapper;

public class JacksonParser {
    public static void main(String[] args) throws IOException {
        String jsonResponse = "{ \"login\": \"octocat\", \"id\": 1 }"; // Replace with actual response

        ObjectMapper mapper = new ObjectMapper();
        JsonNode rootNode = mapper.readTree(jsonResponse);

        String login = rootNode.path("login").asText();
        int id = rootNode.path("id").asInt();

        System.out.println("Login: " + login);
        System.out.println("ID: " + id);
    }
}
import com.google.gson.JsonObject;
import com.google.gson.JsonParser;

public class GsonParser {
    public static void main(String[] args) {
        String jsonResponse = "{ \"login\": \"octocat\", \"id\": 1 }"; // Replace with actual response

        JsonObject jsonObject = JsonParser.parseString(jsonResponse).getAsJsonObject();

        String login = jsonObject.get("login").getAsString();
        int id = jsonObject.get("id").getAsInt();

        System.out.println("Login: " + login);
        System.out.println("ID: " + id);
    }
}
HttpRequest request = HttpRequest.newBuilder()
        .uri(URI.create(url))
        .header("Accept", "application/vnd.github.v3+json")
        .header("Authorization", "Bearer YOUR_PERSONAL_ACCESS_TOKEN")
        .build();
**Solution 37:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
javac HelloWorld.java
javap -c HelloWorld
Compiled from "HelloWorld.java"
public class HelloWorld {
  public HelloWorld();
    Code:
       0: aload_0
       1: invokespecial #1    // Method java/lang/Object."<init>":()V
       4: return
  public static void main(java.lang.String[]);
    Code:
       0: getstatic     #2    // Field java/lang/System.out:Ljava/io/PrintStream;
       3: ldc           #3    // String Hello, World!
       5: invokevirtual #4    // Method java/io/PrintStream.println:(Ljava/lang/String;)V
       8: return
}
**Solution 38:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
javac HelloWorld.java
java -jar cfr-0.152.jar HelloWorld.class --outputdir ./decompiled

**Solution 39:
public class Sample {
    public void greet(String name) {
        System.out.println("Hello, " + name + "!");
    }

    private void secret() {
        System.out.println("This is a secret method.");
    }
}
import java.lang.reflect.Method;

public class ReflectionExample {
    public static void main(String[] args) {
        try {
            // Load the Sample class
            Class<?> clazz = Class.forName("Sample");

            // List all declared methods
            Method[] methods = clazz.getDeclaredMethods();
            for (Method method : methods) {
                System.out.println("Method: " + method.getName());
            }
        } catch (ClassNotFoundException e) {
            e.printStackTrace();
        }
    }
}
import java.lang.reflect.Method;

public class ReflectionExample {
    public static void main(String[] args) {
        try {
            // Load the Sample class
            Class<?> clazz = Class.forName("Sample");

            // Create an instance of Sample
            Object sampleInstance = clazz.getDeclaredConstructor().newInstance();

            // Invoke the public greet method
            Method greetMethod = clazz.getDeclaredMethod("greet", String.class);
            greetMethod.invoke(sampleInstance, "Alice");

            // Invoke the private secret method
            Method secretMethod = clazz.getDeclaredMethod("secret");
            secretMethod.setAccessible(true); // Allow access to private method
            secretMethod.invoke(sampleInstance);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
**Solution 40:
public class VirtualThreadExample {
    public static void main(String[] args) {
        for (int i = 0; i < 100_000; i++) {
            Thread.startVirtualThread(() -> {
                // Simulate task
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {
                    Thread.currentThread().interrupt();
                }
            });
        }
    }
}
**Solution 41:
import java.util.concurrent.Callable;

public class MyTask implements Callable<String> {
    @Override
    public String call() throws Exception {
        // Simulate a task by sleeping for 2 seconds
        Thread.sleep(2000);
        return "Task Completed";
    }
}
import java.util.concurrent.*;

public class ExecutorServiceExample {
    public static void main(String[] args) {
        // Create a fixed thread pool with 5 threads
        ExecutorService executor = Executors.newFixedThreadPool(5);

        // Submit 10 tasks
        List<Future<String>> results = new ArrayList<>();
        for (int i = 0; i < 10; i++) {
            results.add(executor.submit(new MyTask()));
        }

        // Retrieve and print the results
        for (Future<String> future : results) {
            try {
                // This will block until the result is available
                System.out.println(future.get());
            } catch (InterruptedException | ExecutionException e) {
                e.printStackTrace();
            }
        }

        // Shut down the executor
        executor.shutdown();
    }
}
ANSI SQL Using MySQL Exercises
Database Schema
1. User Upcoming Events
List all upcoming events a user is registered for in their city, sorted by date.
SELECT e.title, e.city, e.start_date
FROM Users u
JOIN Registrations r ON u.user_id = r.user_id
JOIN Events e ON r.event_id = e.event_id
WHERE e.status = 'upcoming' AND u.city = e.city
ORDER BY e.start_date;
2. Top Rated Events
Identify events with the highest average rating, considering only those that have received at least 10 feedback submissions.
SELECT e.title, AVG(f.rating) AS avg_rating, COUNT(f.feedback_id) AS feedback_count
FROM Events e
JOIN Feedback f ON e.event_id = f.event_id
GROUP BY e.event_id, e.title
HAVING COUNT(f.feedback_id) >= 10
ORDER BY avg_rating DESC;

3. Inactive Users
Retrieve users who have not registered for any events in the last 90 days.SELECT u.*
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id AND r.registration_date >= CURDATE() - INTERVAL 90 DAY
WHERE r.registration_id IS NULL;
4. Peak Session Hours
Count how many sessions are scheduled between 10 AM to 12 PM for each event.SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
WHERE TIME(s.start_time) >= '10:00:00' AND TIME(s.start_time) < '12:00:00'
GROUP BY e.title;
5. Most Active Cities
List the top 5 cities with the highest number of distinct user registrations.SELECT u.city, COUNT(DISTINCT r.user_id) AS user_count
FROM Users u
JOIN Registrations r ON u.user_id = r.user_id
GROUP BY u.city
ORDER BY user_count DESC
LIMIT 5;
6. Event Resource Summary
Generate a report showing the number of resources (PDFs, images, links) uploaded for each event.SELECT e.title,
       SUM(CASE WHEN r.resource_type = 'pdf' THEN 1 ELSE 0 END) AS pdf_count,
       SUM(CASE WHEN r.resource_type = 'image' THEN 1 ELSE 0 END) AS image_count,
       SUM(CASE WHEN r.resource_type = 'link' THEN 1 ELSE 0 END) AS link_count
FROM Events e
LEFT JOIN Resources r ON e.event_id = r.event_id
GROUP BY e.title;
7. Low Feedback Alerts
List all users who gave feedback with a rating less than 3, along with their comments and associated eventSELECT u.full_name, e.title AS event_title, f.rating, f.comments
FROM Feedback f
JOIN Users u ON f.user_id = u.user_id
JOIN Events e ON f.event_id = e.event_id
WHERE f.rating < 3;
8. Sessions per Upcoming Event
Display all upcoming events with the count of sessions scheduled for them.SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
LEFT JOIN Sessions s ON e.event_id = s.event_id
WHERE e.status = 'upcoming'
GROUP BY e.title;
9. Organizer Event Summary
For each event organizer, show the number of events created and their current status (upcoming, completed, cancelled).SELECT u.full_name, e.status, COUNT(e.event_id) AS event_count
FROM Users u
JOIN Events e ON u.user_id = e.organizer_id
GROUP BY u.full_name, e.status;
10. Feedback Gap
Identify events that had registrations but received no feedback at all.
SELECT e.title
FROM Events e
JOIN Registrations r ON e.event_id = r.event_id
LEFT JOIN Feedback f ON e.event_id = f.event_id
WHERE f.feedback_id IS NULL
GROUP BY e.title;
11. Daily New User Count
Find the number of users who registered each day in the last 7 days.
SELECT registration_date, COUNT(user_id) AS user_count
FROM Users
WHERE registration_date >= CURDATE() - INTERVAL 7 DAY
GROUP BY registration_date;
12. Event with Maximum Sessions
List the event(s) with the highest number of sessions.
SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
GROUP BY e.title
ORDER BY session_count DESC
LIMIT 1;
13. Average Rating per City
Calculate the average feedback rating of events conducted in each city.
 e.city, AVG(f.rating) AS avg_rating
FROM Events e
JOIN Feedback f ON e.event_id = f.event_id
GROUP BY e.city;
15. Most Registered Events
List top 3 events based on the total number of user registrations.
Stack Overflow
SELECT e.title, COUNT(r.user_id) AS registration_count
FROM Events e
JOIN Registrations r ON e.event_id = r.event_id
GROUP BY e.title
ORDER BY registration_count DESC
LIMIT 3;
15. Event Session Time Conflict
Identify overlapping sessions within the same event (i.e., session start and end times that conflict).
SELECT s1.session_id AS session1_id, s2.session_id AS session2_id, s1.event_id
FROM Sessions s1
JOIN Sessions s2 ON s1.event_id = s2.event_id AND s1.session_id < s2.session_id
WHERE s1.start_time < s2.end_time AND s2.start_time < s1.end_time;
16. Unregistered Active Users
Find users who created an account in the last 30 days but haven’t registered for any events.
SELECT u.*
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id
WHERE u.registration_date >= CURDATE() - INTERVAL 30 DAY AND r.registration_id IS NULL;
17. Multi-Session Speakers
Identify speakers who are handling more than one session across all events.
SELECT speaker_name, COUNT(session_id) AS session_count
FROM Sessions
GROUP BY speaker_name
HAVING COUNT(session_id) > 1;
18. Resource Availability Check
List all events that do not have any resources uploaded.
SELECT e.title
FROM Events e
LEFT JOIN Resources r ON e.event_id = r.event_id
WHERE r.resource_id IS NULL;
19. Completed Events with Feedback Summary
For completed events, show total registrations and average feedback rating.
SELECT e.title, COUNT(DISTINCT r.user_id) AS total_registrations, AVG(f.rating) AS avg_rating
FROM Events e
LEFT JOIN Registrations r ON e.event_id = r.event_id
LEFT JOIN Feedback f ON e.event_id = f.event_id
WHERE e.status = 'completed'
GROUP BY e.title;
20. User Engagement Index
For each user, calculate how many events they attended and how many feedbacks they submitted.
SELECT u.full_name,
       COUNT(DISTINCT r.event_id) AS events_attended,
       COUNT(DISTINCT f.feedback_id) AS feedbacks_submitted
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id
LEFT JOIN Feedback f ON u.user_id = f.user_id
GROUP BY u.full_name;
21. Top Feedback Providers
List top 5 users who have submitted the most feedback entries.
CT u.full_name, COUNT(f.feedback_id) AS feedback_count
FROM Users u
JOIN Feedback f ON u.user_id = f.user_id
GROUP BY u.full_name
ORDER BY feedback_count DESC
LIMIT 5;
23. Duplicate Registrations Check
Detect if a user has been registered more than once for the same event.
SELECT user_id, event_id, COUNT(*) AS registration_count
FROM Registrations
GROUP BY user_id, event_id
HAVING COUNT(*) > 1;
23. Registration Trends
Show a month-wise registration count trend over the past 12 months.
SELECT DATE_FORMAT(registration_date, '%Y-%m') AS month, COUNT(*) AS registration_count
FROM Registrations
WHERE registration_date >= CURDATE() - INTERVAL 12 MONTH
GROUP BY month
ORDER BY month;
24. Average Session Duration per Event
Compute the average duration (in minutes) of sessions in each event.
SELECT e.title, AVG(TIMESTAMPDIFF(MINUTE, s.start_time, s.end_time)) AS avg_duration_minutes
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
GROUP BY e.title;
25. Events Without Sessions
List all events that currently have no sessions scheduled under them.
SELECT e.title
FROM Events e
LEFT JOIN Sessions s ON e.event_id = s.event_id
WHERE s.session_id IS NULL;
























