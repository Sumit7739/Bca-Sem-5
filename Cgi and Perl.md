
---

### **Common Gateway Interface (CGI): Introduction**

- **CGI** is a standard way for web servers (like Apache) to communicate with programs. It’s used to **dynamically generate web content**.
- Example: When you fill out a form on a website, CGI takes the input, processes it (via a program like PERL), and sends a response back to the browser.

---

### **CGI URL Interpreted by Web Server**

- When a user interacts with a web page (e.g., clicking "Submit"), the server looks at the **CGI URL** to find the program/script (like a PERL script) to run.
- Example URL:
    
    ```
    http://example.com/cgi-bin/script.pl?name=John&age=30
    ```
    
    - `cgi-bin/script.pl`: The location of the CGI script.
    - `name=John&age=30`: Data sent to the script (query string).

---

### **CGI Program Format**

- A CGI program is a script (often in PERL) that outputs **HTML** for the browser.
- **Example in PERL**:
    
    ```perl
    #!/usr/bin/perl
    print "Content-type: text/html\n\n";  # Tells the browser to expect HTML
    print "<html><body>Hello, World!</body></html>";
    ```
    

---

### **PERL Basics**

**PERL (Practical Extraction and Reporting Language)** is often used for CGI because it’s great for text manipulation and quick scripts.

#### **PERL String Basics**

- Strings in PERL can use single `'` or double `"` quotes:
    
    ```perl
    $string1 = 'Hello';
    $string2 = "World\n";  # Double quotes allow special characters like \n (new line)
    print "$string1 $string2";
    ```
    

---

### **Variables in PERL**

PERL uses **three types of variables**:

1. **Scalars (`$`)**: Hold single values (strings or numbers).
    
    ```perl
    $name = "John";
    $age = 25;
    ```
    
2. **Arrays (`@`)**: Hold lists of values.
    
    ```perl
    @colors = ("red", "green", "blue");
    ```
    
3. **Hashes (`%`)**: Key-value pairs.
    
    ```perl
    %person = ("name" => "John", "age" => 25);
    ```
    

---

### **Array and Indexed Array**

- **Arrays** are ordered lists. You can access elements by their index (starting at 0).
    
    ```perl
    @fruits = ("apple", "banana", "cherry");
    print $fruits[0];  # Outputs: apple
    ```
    

---

### **Hash Array**

- A hash is a collection of key-value pairs.
    
    ```perl
    %student = ("name" => "Alice", "grade" => "A");
    print $student{"name"};  # Outputs: Alice
    ```
    

---

### **Operators in PERL**

PERL supports many operators:

- Arithmetic: `+`, `-`, `*`, `/`, `%`
- Comparison: `==`, `!=`, `<`, `>`, `<=`, `>=`
- String: `.` (concatenate), `eq` (compare strings)

---

### **Control Statements**

Control statements help you control the flow of your program:

- **`if-else`**:
    
    ```perl
    if ($age > 18) {
      print "Adult";
    } else {
      print "Minor";
    }
    ```
    

---

### **Condition and Looping in PERL**

- **Loops**:
    - `while`:
        
        ```perl
        $i = 0;
        while ($i < 5) {
          print "$i\n";
          $i++;
        }
        ```
        
    - `for`:
        
        ```perl
        for ($i = 0; $i < 5; $i++) {
          print "$i\n";
        }
        ```
        

---

### **Functions in PERL**

1. **String Functions**:
    
    - `length($string)` - Gets the length of a string.
    - `uc($string)` - Converts to uppercase.
    - Example:
        
        ```perl
        print length("Hello");  # Outputs: 5
        print uc("hello");      # Outputs: HELLO
        ```
        
2. **Array Functions**:
    
    - `push(@array, $item)` - Add an item to the end.
    - `pop(@array)` - Remove the last item.
3. **Math Functions**:
    
    - `int($num)` - Gets the integer part of a number.
    - `sqrt($num)` - Calculates the square root.

---

### **Input/Output in PERL**

1. **Input**: Use `<STDIN>` to take user input.
    
    ```perl
    print "Enter your name: ";
    $name = <STDIN>;
    chomp($name);  # Removes newline character
    print "Hello, $name!";
    ```
    
2. **Output**: Use `print` to display information.
    

---

### **File Handling in PERL**

1. Open and read/write to files:
    
    ```perl
    open(FILE, ">file.txt") or die "Cannot open file";
    print FILE "Hello, file!";
    close(FILE);
    ```
    

---

### **Directory Management**

- Use `opendir`, `readdir`, and `closedir` to work with directories:
    
    ```perl
    opendir(DIR, ".") or die "Cannot open directory";
    @files = readdir(DIR);
    print "@files\n";
    closedir(DIR);
    ```
    

---

### **Pattern Matching (Regex)**

PERL is famous for **regex (regular expressions)**. Use `=~` for matching.

- Example:
    
    ```perl
    $text = "Hello World";
    if ($text =~ /World/) {
      print "Match found!";
    }
    ```
    

---

### **Subroutine (Function)**

- **Creating a Subroutine**:
    
    ```perl
    sub greet {
      print "Hello!\n";
    }
    greet();
    ```
    
- **Passing Arguments**:
    
    ```perl
    sub add {
      my ($a, $b) = @_;
      return $a + $b;
    }
    print add(5, 3);  # Outputs: 8
    ```
    

---

### **Library in PERL**

PERL has many built-in modules (libraries) for various tasks.

- To use a library:
    
    ```perl
    use Math::Complex;
    print sqrt(-4);  # Outputs: 2i
    ```
    

---

### **Object-Oriented Programming (OOP) in PERL**

PERL supports OOP. You can create classes and objects.

- Example:
    
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
      print "I am a " . $self->{name} . "\n";
    }
    
    my $dog = Animal->new("Dog");
    $dog->speak();  # Outputs: I am a Dog
    ```
    

---

### **PERL Package and Module**

- **Package**: Defines a namespace to avoid name conflicts.
- **Module**: A reusable package stored in a `.pm` file.
    - Example:
        
        ```perl
        package MyModule;
        sub hello {
          print "Hello from MyModule\n";
        }
        1;  # Indicates successful loading
        ```
        

---


Next -> [[CGI and PERL Summary]]