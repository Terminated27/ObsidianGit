A C program implements two threads:
1. The following thread1 waits for an input event on a pin
pthread_mutex_lock(&lock); // Lock during waiting
int interrupt;
interrupt = epoll_wait(epfd, &events, 1,1000);
printf("Event Detected");
pthread_mutex_unlock(&lock); // Unlock after event detected

2. The other thread2 just prints the text of absence of an event to the terminal
printf("Event is NOT Detected");
What would happen if the input event never occurs? Select all that apply. You will get a partial grade for a right choice, and there is negative marking for wrong choices.
  

a.

Mutex lock acquired by thread1 will be unlocked after 1 second

b.

Mutex lock acquired by thread1 will be unlocked after 1000 seconds  

c.

Mutex lock is never acquired by thread1

d.

The program prints "Event detected" and "Event is NOT detected" on the terminal in any order

e.

Mutex lock acquired by thread1 will never be unlocked

a. Mutex lock acquired by thread1 will be unlocked after 1 second

b. Mutex lock acquired by thread1 will be unlocked after 1000 seconds  

e. Mutex lock acquired by thread1 will never be unlocked