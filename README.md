# BoundedBuffer
Colby Morris
ccolbymorris@gmail.com
*******************PURPOSE***********************
This is a program designed to show different threads running simultaneously.
I have created two consumer threads and two producer threads. Once the 
program is running it will output every time a thread produces a number
and every time a thread consumes that number. It will also determine if the
number that was produced is a prime number.

*****************IMPLEMENTATION*****************
Included in this repository is the source code of the java program. To view
the code, click on the src folder. To run the program, simply compile it
using the "javac" command and run it with the java command followed by 
"Server.java", the main class of the program.

*******************LIBRARIES**********************
This program contains four different classes. The "Server.java" class is the
main class and this is where the producer and consumer threads are created
and the threads are started. Inside the Producer.java class is where the
producer threads are bounded to a boundedbuffer. It also comes up with a 
random integer and stores it into the boundedbuffer. The Consumer.java class
takes the integer that the producer thread put into the bounded buffer and 
checks to see if it is a prime number. If it is, it returns true; otherwise it
returns false. Finally, the BoundedBuffer.java class contains methods for accessing
and inputting numbers into a buffer.

***********************API*************************
BoundedBuffer.java
  -public BoundedBuffer()
  //constructor to set values to zero
  
  -public void enter(Object item)
  //method to enter an integer into the buffer
  
  -public Object remove()
  //method to remove an integer from the buffer
  
Consumer.java extends thread
  -public static boolean isPrime(int Number)
  //method which takes an integer as a parameter and outputs true if it is a
  //prime number and false otherwise.
  
  -public void run()
  //method to output that the consumer thread consumed and whether or not it was
  //a prime number
  
Producer.java extends thread
  -public void run()
  //method to create a random number and store it in the bounded buffer
  
  
