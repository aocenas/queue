Original code from Mike Bostock (https://github.com/mbostock/queue).

Only change is that you can add more than one callback with queue.await and
queue.awaitAll and all will be executed after all defered functions finished.
However this means that reusing a queue is a bit harder as all those
callbacks will live within that queue. Maybe adding a reset() function
would be a good idea. 

