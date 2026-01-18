## Concepts
- Backup tools are designed for backing up and restoring data-- helps with loss and data corruption
- 3 popular tools for this-- rsync, deja dup, and duplicity
- We're able to enable auto-synchronization using rsync, you can use a combination of cron and rsync to automate the synchronization process

## Commands
- rsync -- tool to backup and restore data

## Examples
- rsync -av /path/to/mydirectory user@backup_server:/path/to/backup/directory -- copies the entire directory to a remote host
- rsync -avz -e ssh /path/to/mydirectory user@backup_server:/path/to/backup/directory -- data transfer between our local host and the backup server occurs over the encrypted SSH connection

## Answers