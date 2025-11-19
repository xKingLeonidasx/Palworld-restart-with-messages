Server Restart Scripts

This repository contains a collection of Windows batch scripts used to broadcast restart warnings to players and safely restart the server.

📂 Files

Restart server msg 1 min.bat

Sends a broadcast message that the server will restart in 1 minute.


Restart server msg 5 min.bat

Sends a broadcast message that the server will restart in 5 minutes.


Restart server msg 10 min.bat

Sends a broadcast message that the server will restart in 10 minutes.


Restart server.bat

Stops the running server by force-killing the process:

taskkill /im "PalServer-Win64-Test-Cmd.exe" /f

You can extend this file to restart the server after killing the task, or chain it with the message scripts.

🛠 Usage

Run the scripts manually or automate them via Task Scheduler or another automation tool.

Example sequence:

1. Run Restart server msg 10 min.bat

2. Run Restart server msg 5 min.bat

3. Run Restart server msg 1 min.bat

4. Run Restart server.bat to stop the server

📌 Notes

All scripts assume ARRCON is installed in C:\Scripts\ARRCON-3.3.x. Adjust paths if needed.

You can customize the broadcast messages inside each .bat file.

Output messages are intended for in-game player notifications.
