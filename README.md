Disk Scheduling Algorithms in Operating Systems

Overview

This project implements various Disk Scheduling algorithms in Java to simulate how an operating system schedules disk I/O requests. Disk scheduling helps optimize the movement of the disk arm to reduce seek time, improving overall system performance.

Features

Implementation of different disk scheduling algorithms:

First Come First Serve (FCFS)

Shortest Seek Time First (SSTF)

Scan (Elevator Algorithm)

C-Scan (Circular Scan)

Look

C-Look

Graphical or command-line output to visualize the movement of the disk arm.

Input handling for custom disk request sequences.

Technologies Used

Java (JDK 8+)

Java Collections Framework for data handling

Installation

Clone the repository:

git clone 

Navigate to the project directory:

cd disk-scheduling

Compile the Java files:

javac DiskScheduling.java

Run the program:

java DiskScheduling

Usage

The program prompts the user to enter:

The number of disk requests

The request sequence (list of cylinder requests)

The initial position of the disk arm

The scheduling algorithm to be used

After processing, the program outputs the order of execution and the total seek time.

Example Output

Enter the number of requests: 5
Enter request sequence: 98 183 37 122 14
Enter initial head position: 53
Choose a scheduling algorithm: SSTF
Order of execution: 37 -> 14 -> 98 -> 122 -> 183
Total seek time: 236

File Structure

📂 disk-scheduling
├── src
│   ├── DiskScheduling.java
│   ├── FCFS.java
│   ├── SSTF.java
│   ├── SCAN.java
│   ├── C_SCAN.java
│   ├── LOOK.java
│   ├── C_LOOK.java
│   ├── utils
│   │   ├── InputHandler.java
│   │   ├── OutputFormatter.java
├── README.md

Future Enhancements

GUI implementation using JavaFX or Swing

Multi-threaded simulation

Integration with a real-time disk scheduling system

Contributing

Contributions are welcome! Please follow these steps:

Fork the repository.

Create a new branch (git checkout -b feature-name).

Commit your changes (git commit -m 'Add feature').

Push to the branch (git push origin feature-name).

Open a Pull Request.

License

This project is licensed under the MIT License - see the LICENSE file for details.
