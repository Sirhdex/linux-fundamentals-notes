## Concepts
- Once in Linux systems; key targets (configuration files, created scripts, and files / folders)

## Commands
- which-- determine if specific programs are available on OS; searches in PATH
- find-- find files and folders; narrow seraches with parameters
- sudo-- root permission
- locate-- faster find; less parameters

## Examples
- which [python]
- find -type f -name *.conf -user root -size +20k -newermt 2020-03-03 -exec ls -al {} \; 2>/dev/null
- locate *.conf

## Answer
- find / -type f -name *.conf -size -28k -size +25k -newermt 2020-03-03 -exec ls -al {} \; 2>/dev/null
- find / -type f -name *.baf 2>/dev/null | wc -l
- locate xxd