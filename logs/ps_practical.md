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

## Section 2: Finding the Password

### Raspberry Pi Ping Results

```
Pinging raspberrypi.local [192.168.1.187] with 32 bytes of data: 
Reply from 192.168.1.187: bytes=32 time=30ms TTL=64
Reply from 192.168.1.187: bytes=32 time=26ms TTL=64
Reply from 192.168.1.187: bytes=32 time=28ms TTL=64
Reply from 192.168.1.187: bytes=32 time=8ms TTL=64
Reply from 192.168.1.187: bytes=32 time=2ms TTL=64

Ping statistics for 192.168.1.187:
    Packets: Sent = 5, Received = 5, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 2ms, Maximum = 30ms, Average = 18ms
```