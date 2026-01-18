## Concepts
- Filtering texts is very powerful and becoming familiar with it in the long run will help us in terms of navigation
- Great for cutting through large texts to get exactly what we want

## Commands
- more -- automiatically starts file at the start; goes down
- less -- automiatically starts files at the end; goes up
- grep -v -- exclusion option; remove matching lines
- head -- gives us first 10 pages of document
- tail -- gives us last 10 pages of document
- sort -- sorts numerically or alphabetically
- cut -- remove specific delimiters
- tr -- replace characters with ones defined by us
- column -- sorts into columns
- awk -- allows printing specific portions of the text
- sed -- stream editior; most common use is substitution
- ps -- prints snapshot of our current processes
- ps aux -- prints all of processes for all users

## Examples
- cat /etc/passwd | more
- less /etc/passwd
- head /etc/passwd
- tail /etc/passwd
- cat /etc/passwd | sort
- cat /etc/passwd | grep -v "false\|nologin" -- using grep to exclude all who have disabled the standard shell
- cat /etc/passwd | grep -v "false\|nologin" | cut -d ":" -f 1 -- the d option cut off at that limiter, f option gives us the first position of our output
- cat /etc/passwd | grep -v "false\|nologin | tr ":" " "
- cat /etc/passwd | grep -v "false\|nologin | tr ":" " " | awk '{print $1, $NF}' -- prints first and last positions of output

## Answers
- netstat -l | grep '0.0.0.0' | wc -l
- ps aux
- curl https://www.inlanefreight.com | grep https://www.inlanefreight.com -- fetching website contents, then prints specific instances of website
- grep https://www.inlanefreight.com | tr “ “ “\n” | sort -u | grep -E ‘src|href’ | sort -u | wc -l -- searches for and counts specific URLs 
