# Synchronizing Multi Threading java

### Synchronization in java is the capability to control the access of multiple threads to any shared resource.
### Java Synchronization is better option where we want to allow only one thread to access the shared resource.

In this code, there are 2 people Raj and Simran accessing a common resource account, where 1000 balance is stored.
If raj takes out 700 and the thread switch and asks Simran to enter the amount without checking the balance remaining, the system will be corrupted.
         Raj withdraws 700, and if Simran pulls a request for 600, the remaining balance will be -300.
         
         ![before sync](beforeSync.png)


         So we use the synchronized block, so that first Thread t1 is completed then only t2 will run...
         
         ![after sync](https://github.com/peropranav/Synchronizing-Multi-Threading-java/blob/master/afterSync.png)
