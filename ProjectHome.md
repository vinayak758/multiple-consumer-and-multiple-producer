This projects provides one c implementation of multiple producer and multiple consumer problems.

Features:
1. Multiple producer and multiple producer
2. The consumer will submit his request to request queue, and   wait for the response from the producer(implemented via a conditional variable when submitted the request).
3. The producer will inform the proper consumer by wake the proper consumer ID(via the thread ID when customer submitted the request).
4. The shared buffer is a linked list, without lock when reading, but proteced for every node when modifying the count.
5. Require the pthread library.

> Compile command: gcc -g -o0 -o test logger.c vserv.c -lpthread
> To execute: ./test

> Please see the attached documents for more details and send your questions to guixi.zou@gmail.com.