## Concepts
- Daemons are serviecs that provide additional functionailty while running silently in the background
- Generally 2 categories-- System Services and User-Installed Services
- System Services -- internal services needed for system startup
- User-Installed Services -- services added by users
- Daemons are identified by the "d" at the end of the program name
- PID assigend to all processes; viewed in /proc


## Commands
- systemctl start [command] -- starts the designated service
- systemctl status [command] -- checks to see if service has started without error
- systemctl enable [command] -- runs after startup; adds service to SysV
- systemctl list-units --type=service -- lists all services
- journalctl -- view logs; useful if service happens to fail upon startup
- kill -- control and interact with processes
- jobs -- lists all background processes taking place
- fg -- push background process into the foreground

## Examples
- systemd -- first service that starts during the boot process; assigned PID (Process ID)
- kill -l -- lists all signals
- SIGHUP -- sent to process when terminal closes
- SIGINT -- sent when intruptions are sent through terminal
- SIGQUIT -- sent when user quits a process
- SIGKILL -- immidiately kill process
- SIGTERM -- program termination
- SIGSTOP -- stops a program-- won't handle anymore
- SIGTSTP -- sent when user request program suspension

## Answers
- systemctl | grep Load