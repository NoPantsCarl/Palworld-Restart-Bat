### Setting up `start_server.bat`

1. **Place the startup batch file (`start_server.bat`) in the same directory as your `PalServer-Win64-Test-Cmd.exe`.** For example, if your `PalServer-Win64-Test-Cmd.exe` is located at `\PalServer\Pal\Binaries\Win64`, place the batch file there.

2. **Place `ARRCON.exe` in the same location as the batch file.**

3. **Update `C:\SteamServers\steamapps\common\PalServer\steamcmd.exe` to match the location of your `steamcmd.exe`.**

4. **Change `C:\SteamServers\steamapps\common\PalServer\Pal\Binaries\Win64\PalServer-Win64-Test-Cmd.exe` to match the location of your `PalServer-Win64-Test-Cmd.exe`.**

5. **Add any command line arguments you need for your server after `EpicApp=PalServer -useperfthreads -NoAsyncLoadingThread -UseMultithreadForDS`.**

6. **Ensure IP address `192.0.0.1`, port `25575` for RCON, and admin password match your server configuration.**

7. **Update `C:\SteamServers\steamapps\common\PalServer\Pal\Pal\Saved\SaveGames\` to match the location of your savegames folder.**

8. **Update `C:\Users\NoPantsCarl\Documents\PalWorld_BackUps` to where you want the backups to be located.**

9. **Update `D:\PalWorld_BackUps` to the location where you'd like your secondary backups in case the primary location fails.**

10. **Replace `Your Discord Webhook URL` with your actual Discord webhook URL.**

11. **Customize `Server One Is Online` and `Server One 5 Min Warning` to the desired messages for your Discord webhook.**

12. **Adjust the duration of the server restart by changing the `timeout` value (in seconds) after `timeout /t 14400`. For example, for an 8-hour restart, set it to `timeout /t 14400`.**

13. **Optionally, adjust the timeout duration after server boot on line 14 (`timeout /t 120`). The default is 120 seconds, allowing time for the server to initialize before players join.**

#### Requirements
1. [ARRCON](https://github.com/radj307/ARRCON)
2. [7-Zip](https://www.7-zip.org/)
3. Running Windows and not Linux.

#### Note
If you don't want to use Discord webhooks, you can remove line 14 (`timeout /t 120`) and all the other lines that start with `curl`.

Feel free to reach out if you need further assistance! I might update this guide to be clearer in the future!
