## Concepts
- Think of permissions as keys-- you need the correct key to even open the door, let alone obtain the contents inside
- We typically have 3 permissions-- read, write, and execute
- Permissions can be set to 3 things-- group, owner, and others
- SUID / SGID -- allows placing of special permissions on files
- Sticky Bits allow for only certain people to even change permissions-- extra security layer

## Commands
- chmod [-u (owner), -g (group), -o (others), -a (all users)] -- modify permissions
- chmod a+r [directory / file] && ls -l-- changes permissions, while also listing the permissions if the first statement was true
- chown [user:group] [file  directory] -- changes the owner / group of a file / directory


## Examples
- drw-rw-r-- -- how permissions are dictated within our terminal
- chown root:root shell && ls -l -changes the owner of the associated file to root
