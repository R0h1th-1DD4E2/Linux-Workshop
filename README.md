## Bash Scripting

### Shebang
`#!/bin/bash` - This tells the system that the script should be run with the bash shell.

#### Example
```bash
#!/bin/bash
echo "Hello, World!"
```

### Variables in Bash
```bash
#!/bin/bash 
name="Alice" 
echo "Hello, $name!"
```

### User Input
```bash
#!/bin/bash
echo "What's your name?"
read name
echo "Hello, $name!"
```

### Conditions (if statements)
```bash
#!/bin/bash
echo "Enter a number:"
read num

if [ $num -gt 10 ]; then
  echo "Your number is greater than 10!"
else
  echo "Your number is 10 or less!"
fi
```

### Common Condition Tests:

| Test                                     | Description                                  |
| ---------------------------------------- | -------------------------------------------- |
| `-d <file>`                              | True if `<file>` is a directory.             |
| `-f <file>`                              | True if `<file>` is a regular file.          |
| `-e <file>`                              | True if `<file>` exists.                     |
| `-z <string>`                            | True if `<string>` is empty.                 |
| `-n <string>`                            | True if `<string>` is not empty.             |
| `"<str1>" = "<str2>"`                    | True if strings are equal.                   |
| `"<str1>" != "<str2>"`                   | True if strings are not equal.               |
| `-eq`, `-ne`, `-lt`, `-le`, `-gt`, `-ge` | Numeric comparisons.                         |
| `!`                                      | Negates the condition (logical NOT).         |
| `&&`                                     | Logical AND (both conditions must be true).  |
| \|\|                                     | Logical OR (any one conditions can be true). |

### Loops 

#### For Loop
```bash
#!/bin/bash
for i in {1..5}
do
  echo "Number: $i"
done
```

#### While Loop
```bash
#!/bin/bash
counter=1
while [ $counter -le 5 ]
do
  echo "Counter: $counter"
  ((counter++))
done
```

### Function
```bash
#!/bin/bash

greet() {
  echo "Hello, $1!"
}

greet "Alice"
greet "Bob"
```

### Comments
```bash
# This is a comment
```