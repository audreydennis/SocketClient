# TCP Socket Client

Write a Java app that will

- Connect to a server (command-line parameter) on a port (2nd command-line parameter)
- Take any input passed on the command line (any command-line parameter beyond 2), send it down the socket
- Capture any output from the socket, print it to the console
- Demonstrate that it works by connecting to:
- server djxmmx.net / port 17 (Quote of the Day service)
- server time.nist.gov / port 13 (Date-and-Time service)
- server tcpbin.com / port 4242 or 34.230.40.69 / port 30000 (Echo service)
- In each case, capture the shell session in a video or text file, and put those files into the GitHub repository containing your code.
 

Bonus points: Logging (2 pts)
- Provide diagnostic logging that describes to the console what is happening (1pt)
- The logging is configurable, displaying different "levels" of logging depending on a command-line flag passed in (2 pts)
- TIP: see java.util.logging

Bonus points: Threading (2 pts)
- Make your client interactive: Users can type at the console and the input goes down the socket
- TIP: you will need to have two Threads:
- one Thread handles command-line I/O (System.in, System.out)
- second Thread handles socket I/O
- Somehow those Threads need to talk to one another
