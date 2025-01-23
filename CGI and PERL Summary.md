
---

### **Common Gateway Interface (CGI)**

1. **Introduction**: CGI is a standard protocol used to enable communication between a web server and a program/script that generates dynamic web content.
2. **CGI URL Interpretation**: A CGI URL specifies the location of the CGI script on the server and includes data (query string) to be passed to the script.
    - Example: `http://example.com/cgi-bin/script.pl?name=John`
3. **CGI Program Format**: A CGI program outputs HTTP headers followed by the content (like HTML).
    - Example in PERL:
        
        ```perl
        print "Content-type: text/html\n\n";
        print "<html><body>Hello, World!</body></html>";
        ```
        

---
****
### **PERL Basics**

1. **Introduction**: PERL (Practical Extraction and Reporting Language) is a high-level programming language, often used for CGI scripts due to its text manipulation capabilities.

---

### **PERL Basics and Data Types**

1. **Strings**: Text enclosed in single `'` or double `"` quotes.
    - Example: `$string = "Hello, World!";`
2. **Variables**: PERL supports:
    - **Scalars (`$`)**: Hold single values (numbers or strings).
    - **Arrays (`@`)**: Hold ordered lists of values.
    - **Hashes (`%`)**: Hold key-value pairs.

---

### **PERL Data Structures**

1. **Array**: An ordered list of elements.
    - Accessed by index starting from 0.
    - Example: `@fruits = ("apple", "banana"); print $fruits[0];`
2. **Hash**: A collection of key-value pairs.
    - Example: `%person = ("name" => "John"); print $person{"name"};`

---

### **Operators in PERL**

1. **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
2. **Comparison Operators**:
    - Numeric: `==`, `!=`, `<`, `>`, `<=`, `>=`
    - String: `eq` (equal), `ne` (not equal)
3. **String Operators**: `.` (concatenation)

---

### **Control Statements**

1. **If-Else Statement**: Used for decision-making.
    - Example:
        
        ```perl
        if ($age > 18) {
          print "Adult";
        } else {
          print "Minor";
        }
        ```
        
2. **Loops**: Used to repeat a block of code.
    - **While Loop**: Executes while a condition is true.
    - **For Loop**: Executes a block for a specified range.

---

### **Functions in PERL**

1. **String Functions**:
    - `length($string)`: Returns the length of a string.
    - `uc($string)`: Converts a string to uppercase.
2. **Array Functions**:
    - `push(@array, $value)`: Adds a value to the end of an array.
    - `pop(@array)`: Removes the last element.
3. **Math Functions**:
    - `int($value)`: Returns the integer part of a number.
    - `sqrt($value)`: Calculates the square root.

---

### **Input/Output in PERL**

1. **Input**: Use `<STDIN>` to get user input.
    - Example: `$name = <STDIN>; chomp($name);`
2. **Output**: Use `print` to display data.

---

### **File Handling in PERL**

1. **Opening Files**: Use `open` to work with files.
    - Example:
        
        ```perl
        open(FILE, ">output.txt") or die "Cannot open file";
        print FILE "Hello, World!";
        close(FILE);
        ```
        

---

### **Directory Management**

1. **Working with Directories**: Use `opendir`, `readdir`, and `closedir`.
    - Example:
        
        ```perl
        opendir(DIR, ".") or die "Cannot open directory";
        @files = readdir(DIR);
        closedir(DIR);
        ```
        

---

### **Pattern Matching in PERL**

1. **Regex Matching**: Used for searching and replacing text.
    - Example: `$text =~ /pattern/` checks if `pattern` exists in `$text`.

---

### **Subroutines in PERL**

1. **Definition**: Subroutines are user-defined functions.
    - Example:
        
        ```perl
        sub greet {
          print "Hello!";
        }
        greet();
        ```
        
2. **Arguments**: Values can be passed to subroutines.
    - Example:
        
        ```perl
        sub add {
          my ($a, $b) = @_;
          return $a + $b;
        }
        print add(5, 3);
        ```
        

---

### **Libraries and Modules**

1. **Library**: Built-in or external reusable code (e.g., `Math::Complex`).
    - Example: `use Math::Complex;`
2. **Module**: A reusable package, typically stored as a `.pm` file.

---

### **Object-Oriented Programming in PERL**

1. **Introduction**: PERL supports OOP concepts like classes, objects, and methods.
2. **Example**:
    
    ```perl
    package Animal;
    sub new {
      my $class = shift;
      my $self = { name => shift };
      bless $self, $class;
      return $self;
    }
    sub speak {
      my $self = shift;
      print "I am a " . $self->{name};
    }
    my $dog = Animal->new("Dog");
    $dog->speak();
    ```
    

---

### **PERL Package and Module**

1. **Package**: A namespace for organizing code and avoiding name conflicts.
    - Example:
        
        ```perl
        package MyPackage;
        sub say_hello {
          print "Hello!";
        }
        1;  # Indicates successful loading
        ```
        
2. **Module**: A file containing a package, usually ending in `.pm`.

---

Next -> [[Database Connectivity]]