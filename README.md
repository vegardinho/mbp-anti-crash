# MacBook Pro anti crash script.
## What is it?
- Daemon and python3 script for solving sudden crash issue of MacBook Pro models 2013-2015. (See https://www.reddit.com/r/mac/comments/9pyort/apple_macbook_pro_sudden_crash_fix_for_models/ for details.)
- Based on https://www.notebookservice030.de/downloads/mbp/MBP-Anti-CrashLevel1.dmg

## How to install
- Edit follwing keys in properylist-file:
  - `ProgramArguments`: path of the embedded python script.
  - `StandardOutPath`: path of log file.
  - `StandardErrorPath`: path of error log file.
  - `UserName`: name of user that script will run as.
- Place propertylist-file (daemon) in `/Library/LaunchDaemons/`. (This ensures the script will run regardless of logged-in user.)
