

Part 1:

Given two character strings `s1` and `s2`. Write a Pthread program to find out the number of substrings, in string `s1`, that is exactly the same as `s2`. For example, suppose `number_substring(s1, s2)` implements the function, then `number_substring(“abcdab”, “ab”)` = 2, `number_substring(“aaa”, “a”)` = 3, `number_substring(“abac”, “bc”)` = 0. The size of `s1` and `s2` (`n1` and `n2`) as well as their data are input by users. Assume that `n1` mod NUM_THREADS = 0 and `n2 < n1/NUM_THREADS`.



Part 2:

Using condition variables to implement a producer-consumer algorithm. Here we have two threads: one producer and one consumer. The producer reads characters one by one from a string stored in a file named “message.txt”, then writes sequentially these characters into a circular queue. Meanwhile, the consumer reads sequentially from the queue and prints them in the same order. Assume a buffer (queue) size of 5 characters. Write a Pthread program using conditional variables.