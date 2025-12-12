# PS Practical

i have opened the repo and started my log!!!

# Cheese Problem Found

the problematic commit was **2ded3c2bfb756cd031436fca89a82ca0736e2138** with message "Do something again".

**Issues found:**
- `import java.io.FileCheeseStream;` replaced `FileOutputStream`
- `scanner.cheese()` replaced `scanner.nextLine()`
- `} cheese (` replaced `} catch (`
- `byte[] cheese` replaced `byte[] passwordBytes`

all intances of "cheese" were replacing  java code in the ReversibleEncryptor.java file.