CSC 252 - Program 5 - Pirority Queues, Binary Heaps & Union by LaNadia Bailey
GenAI was used to debug and understand unknown concepts.

This project creates a incident managment system by processing them and putting them in order by priority.

Java Files:
Incident.java - Incidents are ordered by priority, timestamp, ID, and description.
UnionFind.java - Compresses paths, union by ranks, and counting connected segments.
Main.java - Main driver that reads input commands and manages the priority queue of incidents by arranging them in the correct order. 

Example Run:
Input: 10 12
ADD_INCIDENT 1 5 100 Malware alert - LINK(3,7)
ADD_INCIDENT 2 9 101 DDoS detected - CHECK(3,7)
ADD_INCIDENT 3 9 99 Switch failure - LINK(2,9)
PEEK_NEXT
PROCESS_NEXT
SAME_SEGMENT 3 7
PROCESS_NEXT
SAME_SEGMENT 3 7
PROCESS_NEXT
SAME_SEGMENT 2 9
SEGMENT_COUNT
PROCESS_NEXT
Output: Incident{id = 2, priority = 9, timestamp = 101, description = "DDoS detected - CHECK(3,7)"}
Incident{id = 2, priority = 9, timestamp = 101, description = "DDoS detected - CHECK(3,7)"}
NO
NO
Incident{id = 3, priority = 9, timestamp = 99, description = "Switch failure - LINK(2,9)"}
NO
Incident{id = 1, priority = 5, timestamp = 100, description = "Malware alert - LINK(3,7)"}
YES
12
EMPTY
