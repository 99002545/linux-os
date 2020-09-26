# linux-os

makefile:
all:
	gcc food.c -pthread -o all
clean:

to run:
make
./all

description of my code:

I implement the semaphore and mutex in my code.
I take the maximum items = 7 and the buffer items =7.
there is 2 function named as chef and customer.
the chef order the item and after that the customer food order is removed.
the mutex works here and created lock and unlock.
A mutex provides mutual exclusion, either producer or consumer can have the key (mutex) and proceed with their work. As long as the buffer is filled by producer, the consumer needs to wait, and vice versa.
At any point of time, only one thread can work with the entire buffer.

semaphore:A semaphore is a generalized mutex. In lieu of single buffer, we can split the 4 KB buffer into four 1 KB buffers (identical resources). A semaphore can be associated with these four buffers. The consumer and producer can work on different buffers at the same time.

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/cc6169000d5b4b228c68c2ed6f3695fd)](https://app.codacy.com/manual/99002545/linux-os?utm_source=github.com&utm_medium=referral&utm_content=99002545/linux-os&utm_campaign=Badge_Grade_Settings)
![cppcheck-action](https://github.com/99002545/linux-os/workflows/cppcheck-action/badge.svg)
![CI](https://github.com/99002545/linux-os/workflows/CI/badge.svg)
![Unit testing](https://github.com/99002545/linux-os/workflows/Unit%20testing/badge.svg)
