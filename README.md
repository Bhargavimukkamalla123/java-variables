# 🧠 Java Variables in Depth

Welcome to my Java learning repository!  
This repo covers all **types of variables in Java** with simple explanations and code examples. 🚀

---

## 📌 What is a Variable?

A **variable** in Java is a container that holds data during program execution. Each variable must be declared with a **type**.

Or simply:

> A **variable** is a placeholder used to store specific types of values such as numbers, characters, or text. These values can be accessed, used, and modified during the program's execution.
>
> 📖 Example:  
```java
int age = 21;
String name = "Bhargavi";

---

🔠 Types of Variables in Java
🧍‍♀️ Instance Variables

🏛️ Class (Static) Variables

📦 Local Variables

📥 Parameters

1.🧍‍♀️ Instance Variables(non-static fields)
🔹 Defined inside the class, but outside any method.
🔹 Belongs to each object.

🧪 Example:
 public class Student {
    int id;
    String name;

    public static void main(String[] args) {
        Student s1 = new Student();
        s1.id = 101;
        s1.name = "Rama";
        System.out.println("Id: " + s1.id);
        System.out.println("Name: " + s1.name);
    }
}


2.🏛️ Class Variables (Static):
🔹 Defined with the static keyword.
🔹 Can be accessed without creating objects.
🧪 Example:
 public class School {
    static String schoolName = "ABC High School";

    public static void main(String[] args) {
        System.out.println("School: " + schoolName);
    }
}

3.📦 Local Variables
🔹 Defined inside methods only outside the class.
🔹 Scope is limited to that method.

🧪 Example:
public class LocalExample {
    public static void main(String[] args) {
        int age = 20;
        System.out.println("Age: " + age);
    }
}
4.📥 Parameters
🔹 Variables passed into a method to receive input.
🔹 Only declared, not initialized in the method signature.

🧪 Example:
public class Greet {
    void sayHello(String name) {
        System.out.println("Hello, " + name);
    }

    public static void main(String[] args) {
        Greet g = new Greet();
        g.sayHello("Bhargavi");
    }
}


🧪 How to Compile & Run:
        javac FileName.java
        java FileName


📊 Summary Table
  Type	              Declared Inside     	 Static Allowed	     Access
-------------------------------------------------------------------------------
🧍‍♀️ Instance       	  Class,outside methods	       ❌	           Object needed
🏛️ Class (static)	    Class, outside methods	     ✅        	   Direct access
📦 Local	            Inside methods	             ❌	           Only in method
📥 Parameters	        In method declaration	       ❌	            From method calls


🧠 Naming Conventions for Variables in Java
1.✅ Variables are case-sensitive

2.✅ Use lowercase for single-word names:
int age = 20;

3.✅ Use camelCase for multi-word names:
String bankAccountNo = "1234";

4.❌ Avoid using class names or Java keywords:
Don’t use String, class, static, etc. as variable names

5.✅ Allowed special characters:
Only _ (underscore) and $ (dollar)



  

