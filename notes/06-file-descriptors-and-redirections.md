## Concepts
- Linux files all have file descriptors, same thing as a Windows file handle
- We can use descriptors as a way to redirect output, input, and errors
- < > are our means of doing so

## Commands
- find / -type f -name *.conf 2>/dev/null -- redirecting errors to /dev/null
- find / -type f -name *.conf 2>/dev/null > results.txt -- directs results into txt file
- find /etc/ -name shadow 2>sterr.txt 1>stopt.txt -- forwarding to two different texts
- find /etc/ -name passwd >> passwd.txt 2>/dev/null -- appends output into txt file
- dpkg -- debian packages

## Examples

## Answers
- find / -type f -name *.log 2>/dev/null | wc -l
- dpkg --list | grep ii | wc -l 