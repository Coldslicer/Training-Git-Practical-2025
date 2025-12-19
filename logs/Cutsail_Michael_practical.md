PING 192.168.1.187 (192.168.1.187): 56 data bytes
Request timeout for icmp_seq 0
Request timeout for icmp_seq 1
Request timeout for icmp_seq 2
Request timeout for icmp_seq 3

Step 6: Cheese replaced certain variables and methods in the file, causing it to run improperly. Commit 8bea32d.\

Step 8: So far, I've replaced the cheese error in ReversibleEncryptor.java. This allows it to run properly again.

--- 192.168.1.187 ping statistics ---
5 packets transmitted, 0 packets received, 100.0% packet loss
PING 192.168.1.187 (192.168.1.187): 56 data bytes
64 bytes from 192.168.1.187: icmp_seq=0 ttl=64 time=74.377 ms
64 bytes from 192.168.1.187: icmp_seq=1 ttl=64 time=40.442 ms
64 bytes from 192.168.1.187: icmp_seq=2 ttl=64 time=3.930 ms
64 bytes from 192.168.1.187: icmp_seq=3 ttl=64 time=4.099 ms
64 bytes from 192.168.1.187: icmp_seq=4 ttl=64 time=4.068 ms

--- 192.168.1.187 ping statistics ---
5 packets transmitted, 5 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 3.930/25.383/74.377/28.266 ms
PING 192.168.1.187 (192.168.1.187): 56 data bytes
64 bytes from 192.168.1.187: icmp_seq=0 ttl=64 time=12.426 ms
64 bytes from 192.168.1.187: icmp_seq=1 ttl=64 time=12.088 ms
64 bytes from 192.168.1.187: icmp_seq=2 ttl=64 time=8.168 ms
64 bytes from 192.168.1.187: icmp_seq=3 ttl=64 time=13.764 ms
64 bytes from 192.168.1.187: icmp_seq=4 ttl=64 time=13.166 ms

--- 192.168.1.187 ping statistics ---
5 packets transmitted, 5 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 8.168/11.922/13.764/1.965 ms
PING 192.168.1.187 (192.168.1.187): 56 data bytes
64 bytes from 192.168.1.187: icmp_seq=0 ttl=64 time=13.582 ms
64 bytes from 192.168.1.187: icmp_seq=1 ttl=64 time=13.232 ms
64 bytes from 192.168.1.187: icmp_seq=2 ttl=64 time=8.341 ms
64 bytes from 192.168.1.187: icmp_seq=3 ttl=64 time=12.849 ms
64 bytes from 192.168.1.187: icmp_seq=4 ttl=64 time=4.322 ms

--- 192.168.1.187 ping statistics ---
5 packets transmitted, 5 packets received, 0.0% packet loss
round-trip min/avg/max/stddev = 4.322/10.465/13.582/3.614 ms

Step 21: I fixed the problems with cheese in the ReversibleEncryptor.java file. Then I found the secret password for it and decryped the file encrypted.txt into a regular image.