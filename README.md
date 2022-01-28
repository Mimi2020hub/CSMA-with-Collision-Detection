# CSMA-with-Collision-Detection

CSMA/CD (CSMA with Collision Detection), a media access control (MAC) method used most notably in early Ethernet technology for local area networking (LAN). It defines how network stations respond when two stations attempt to use a channel simultaneously and encounter a collision. The bus topology is considered where all the nodes are directly connected to a common half-duplex link. When one node sends its signal, other nodes connected to the same link are able to detect it. As for the carrier sensing methods, both 1-persistant and non-persistent carrier sensing are considered.

Revise given code to implement a random back-off algorithm. Please ignore the wait 9.6us and Transmit 48 Jam.
After collision is detected, the backoff time is a float number in original code, while the backoff time is selected by multiplying a random number in the contention window with the time slot 51.2us in the random back-off algorithm. The maximum size of the contention window is 210 = 1024. Meanwhile, the maximum time of collision is 10 in original code, while that is 15 in random back-off algorithm.

Compare the performance of efficiency and throughput for both the code in Project2_CSMACD.py and the code to implement the random back-off algorithm under following cases:
(1) Set the packet delivery rate A = 10. Increase the user number from 20 to 100 every 20. Both 1-persistent and non-persistent carrier sense methods are considered.
(2) Set the user number N = 20. Increase the packet delivery rate from 5 to 20 every 5. Both 1- persistent and non-persistent carrier sense methods are considered.
