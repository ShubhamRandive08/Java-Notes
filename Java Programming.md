
### *What is Java?*
-  Java is an general purpose, high level, interpreted, compiled, static, function oriented, object oriented, platform independent programming language which is used to develop any kind of application.
     `1. General Purpose - With using the JAVA we can develop any kind of applicaiton` <br>
     `2. High Level - Java is also human readable language, which is easily understand to the human` <br>
     `3. Interpreted - In the Java, there are also presents the interpreter to execute the code line by line. And which is also converts the byte code into the machin code` <br>
     `4. Compiled - Java can be also provide the compiler to convert the source into the byte code` <br>
     `5. Functional oriented - In we can also pass the one fucntion to another function as a arguments (Ex, Lambada fucntion)` <br>
     `6. Object oriented - In java, we can also create the object.`<br>

### *What is JRE, JVM, JDK ?*<br>

- These three are main components of the Java. These are also responsible for execute and run the java application.
-  JVM 
   - JVM stands for Java virtual machine. Which is also responsible for the load the byte code with the help of Class loader. Then JVM will verify the code with the help of the code verifier for to check the security of the code. It's also provides the various memory areas like heap, stack, method, PC register program and native areas to store the variables and methods. It also provides the interpreter and execution engines to execute the code line by line and  also boost the performance of the application with the help of JIT. And also remove the unused objects with the help of garbage collection. <br> <br>
-  JDK 
    -    JDK stands for Java Development Kit. Which is also responsible for execute, compile, run the Java program. Without JDK we can't able to compile the code. It also provides the JVM and JRE. <br> <br>
- JRE 
  - JRE stands for Java Runtime environment which is also provide library and predefined class and interfaces to us like System form java.lang.* package. 

`Part of JRE. Provides memory areas, execution engine, garbage collector` <br>
`JVM + Core Libraries (like `java.lang`, `java.util`, `java.io`)`

`JRE + Development Tools (`javac`, debugger, jar, etc.)`

### Why main method is public?
- Because of the JVM can call it. <br><br>
### What is System.out.println() ?

- It is syntax for print any result on the output window. 
- `System` is an class of the java.lang package.
- `out` is an static variable which is present in System class. The datatype of the `out` variable is PrintStream. ( This is Class )
- `println()` is a method which is also present inside the PrintStream class. 
<Br> <br>

### Datatypes in Java
#### Primitive Datatype - 
1. byte
2. short 
3. int 
4. long
5. float
6. double
7. boolen
8. char
<br><br>
#### Non-Primitive Datatype
1. String 
2. Array
3. Class
4. Interface
5. Enum
<br><br>
### Operators in Java :
- Operator is a special symbol which is used to perform the  operations.

1. Arithmetic ( + , - , * , / )
2. Relational ( < , > , <= , >= )
3. Logical ( &&, || , ! )
4. Assignment ( = , += , -= , *= , /= ) 
5. Unary (++, --, )
6. Ternary ( ?   :  ) <br><br>
### Control Flow statement <br>
- It we want to control the program execution flow then we should go for control flow statement
	 1. Conditional statement ( if, if else, else if, nasted if )
	 2. Looping statement ( for, while , do while , nasted for )
	 3. Transfer statement <br><br>
### OOPs <br>
#### What is the OOPs?
- OOPs stands for Object oriented programming.
- It just way to write the program
- OOPs programming also represents the real word entity.
- OOPs programming also based on the class and object concept.
- There are four pilers of OOPs : 1. Abstraction. 2. Polymorphism. 3. Encapsulation. 4. Inheritance.<br><br>
#### What is class?<br>
- Class is the logical entity. Which is also known as a blueprint for the object. Class is a group of variable, methods, constructors as well as block. <br><br>

#### What is the object?<br><br>
- Object is the physical entity.
- Object is the instance of the class.
- Object having states (variable) and behavior (Methods).<br><br>
- ### Anonymus object : This object which is don't have any name. 
      `Ex, new Obj();`

#### What is the reference variable?<br><br>
- It will holds/store the address of the object.<br><br>

#### new keyword<br><br>
- It is the keyword which is also used for allocate the memory to another object.<br><br>

#### What is the method?<br><br>
- Method is a group of the code which is used to perform the certain task.
- Types of method - 1. User defined method 2. Predefined method.<br><br>

#### what is the `this` keyword?<br><br>
- It is used to diffrentiate local variable and globle variable. 
- `this` refers to the global variable.
- And it is used when the local variable and globle variable should be same.<br><br>

#### What is constructor?<br><br>
- Constructor can be used for initialize the object/instance variable.
- Constructor name and class name should be same.
- Class don't contain any return type.
- Constructor can be automatically called when the object is created.
- For each object constructor will call only one time.
- Types of constructor :
        1. Parameterized constructor
        2. Non Parameterized constructor ( Default constructor )
<br><br>
```Copy

public class ConUser{

    ConUser(){ // Non parameterized constructor

        System.out.println("0 Param");

    }

    ConUser(int a, int b){ // Parameterized constructor ( Default constructor )

        System.out.println("2 Params");

    }

    public static void main(String[] args) {

        ConUser con = new ConUser();

        ConUser con2 = new ConUser(12,20);

    }

}
```
<br><br>

```Output
0 Param
2 Params
```

<br><br>
#### Constructor chaining :
- Constructor chaining means call the one constructor from another one within same class or from parent class.
- It is also achive with the help of this() call if the constructor within the same class.
- If the constructor can also present in parent or chind class then this can be achive with the super class.<br><br>

#### Type of variable <br>
- Variable is a container which is used to store the data on computer memory like RAM.<br>

Types of Variable -<br>
  1. Instance variable / Non static variable / Global variable
  2. Static variabel
  3. Local variable<br>

1. Instance variable<br>
- Which variable created inside the class and outside of any method and constructor that variable is called `instance variable`.
- It is also known as global / non static variable.
- Instance variables are related to objects.
- Instance variable value for each object will change.

2. Static variable <br>
- Which variable created with the help of static keyword this is called static variable.
- Static variable value is comman for all objects.
- Static variable is related with class.

3. Local variable
- Which variable is created inside the any method and constructor this is called local variable.
- It is also used for fulfill temporary requirement.
<br>

```Copy

// Can we access the instance variable in instance method : Yes

// Can we access the static variable in instance method : Yes

// Can we access the instance variable in static method : No directly but using Object of class which is indirectly

// Can we access the static variable in static method : Yes

// Static variable is accessible for both like instance method and static method. But instance variable is accessible only the instance method not for static method directly.

public class InstanceVariableStaticVariableConcept {
    int a; // Instance variable / Gloable variabel / Non static variable - Which variable also declare inside the class and outside the any method or constructor. 
    static int b; // Static variable - which variable declare with the static keyword thats call static variable which is also related with the Class directly. Static variabel value is also commann for all object.

    void returnSum(){ 
      int a; // Local variable
        System.out.println("The value of a : " + (a + b));
    }

    static void returnSub(){
        int sum; // Local variable
        System.out.println("The value of b : " + b);
    }
    
    public static void main(String[] args) {
        
    }
}

```










