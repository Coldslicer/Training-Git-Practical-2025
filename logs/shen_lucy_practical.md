I have opened the repo and started my log!” in the log file and commit that change

The problem was in commit 8bea32d

section 1 step 8 summary:
So far what I've done is use vi, git log, git add, git reset

Pinging 192.168.1.187 with 32 bytes of data:
Reply from 192.168.1.187: bytes=32 time=1ms TTL=64
Reply from 192.168.1.187: bytes=32 time=4ms TTL=64
Reply from 192.168.1.187: bytes=32 time=3ms TTL=64
Reply from 192.168.1.187: bytes=32 time=2ms TTL=64

Ping statistics for 192.168.1.187:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 1ms, Maximum = 4ms, Average = 2ms

I committed one more time, and created an original.txt file. Looked into gitignore, saw that .env was on it, so thats why it was not added
