# Kruskal's Algo for clustering datapoints

This assignment was a simple clustering algorithm with Kruskal's shortest path and distance metrics.


## My notes on implementation

Hello, first off, this was a pretty fun assignment. Although, given time contraints, I couldn't spend as much time on it as I would like.

PART 1) - MyGraphTest1.java shows tests run completely.
PART 2) - PartitionTest2.java shows tests run completely.
PART3) - MyGraphTest123.java and Clusters2DTest123.java do not run completely. I explain more of this malfunction below under "Known bugs".

### General Working:
1.) Tests for PartitionTest2.java seem to run well with no bugs
2.) Test for MyGraphTest1.java seem to run well as well with minimal bugs


### Known bugs:
1.)  at java.base/java.util.AbstractQueue.remove(AbstractQueue.java:117)
 - While implementing the Pseudocode for Kruskal's Algo, it highlighted this: ("(u,v)=edge returned by PQ.removeMin()") operation.
 - For some reason I wasn't able to figure out, the removeMin command was not composable with the PQ. I instead use "pq.remove()" which resulted in an error after a few iterations.

2.) at MyGraphTest123.testGraph(MyGraphTest123.java:75)
 - I highlighted earlier that most of my known bugs are in regards to the implementation of Kruskal algo Pseudocode.
 - Due to the same bug pointed out earlier in 1, the test MyGraphTest123 was not able to run completely.

