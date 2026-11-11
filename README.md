# Project 1: My First Nmap Scan

## What I Wanted To Do
I wanted to learn how to find open ports on a computer using Nmap.
I used scanme.nmap.org

## Tools I Used
- Laptop: HP Windows
- Tool: Nmap + Zenmap
- Target:scanme.nmap.org (45.33.32.156)

## Command I Used
nmap -T4 -A -V scanme.nmap.org
* -T4 = Made it fast
* -A = Told me everything, OS version
* -V = Showed me the way it works

## What I Found
| Port | State | Service | Version |
| --- | --- | --- | --- |
| 21 | open | ftp | tcpwrapped |
| 22 | open | ssh | OpenSSH 6.1p1 Ubuntu |
| 80 | open | http | Apache 2.4.7 Ubuntu |
| 9929 | open | nping-echo | Nping echo |

996 other ports were closed. Only 4 were open.

## What it means
- Port 22 is for SSH, where admin logs in. It is using an old version.
- Port 80 is for website. It is using Apache 2.4.7, also old
- The computer is running Linux Ubuntu.
- It took 19 hops for my scan to reach the server, and 59 seconds to finish.

## What I Learned
I learned how to install Nmap, run a scan, read open ports, find OS and service versions, and see traceroute.
