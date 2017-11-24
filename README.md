Log4j: 
Log4j is a framework written in java which is highly configurable. 
Here one question may come that what do we mean by “Framework” ? Framework is nothing but a partially or semi build application. One can use it for building other software.

Log4j is used in java application for writing log in the code. Jar file (or dependency if you use Maven) need to be added to project if you want to use log4j. 

Where to use log4j??

Suppose we are writing code to develop a software. For tracking and debugging our code, we generally write    “system.out.println(“Your message”); “ . So, we will write system.out.println(“Your message”); statement as much as we need. Let's say we have written 100 lines of this statement. 
Now think, release of  first  version of our project has been submitted to our client. We cannot see these “system.out.println(“Your message”); ” statements’ messages at the run time. So there is no chance of tracking our software run with “system.out.println(“Your message”);”. Again before deploying the software in client machine, we have to remove all the statement from the code one by one. It's time consuming. 
Now imagine, after some period your client come to and say that they want another functionality at their software.  So, again you have to put all the “system.out.println(“Your message”);” statements you previously deleted. For doing this, you need to find the exact location in code where this statement should be placed. This is also too much time consuming. Besides this, additional code for additional features will also have additional line of this statement. And again we have to  remove these statements one by one before releasing the Version 2 of the software.

Another problem in using “system.out.println(“Your message”);” statement is that it is synchronized, So it is heavy weight. It makes it expensive and time consuming . 

Now if we have something that may help us to write statements like  “system.out.println(“Your message”);” which may show message at console of our IDE exactly like “system.out.println(“Your message”);” statement and we can disable these statements with a single line of code and enable again with a single line of code then it will be awesome.

Here Log4j comes with a feature like these and have other features too. We can write statement like “system.out.println(“Your message”);” , we call log. We can write these logs into a file, database, etc at the running time as well. We can set log level(total 7 different types) like info, error, warn, debug, fatal, trace  according to the code structure and  message we want to show. 

The best use of log4j is that it can save logs in a file or database. So at the time of running our software at client machine, if it generate any problem then we can just collect the log file and find out the problem. This means, we can track our code even at running time. 


