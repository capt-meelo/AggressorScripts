## AggressorScripts

Collection of scripts that I created to make my life easier since I'm not good at remembering command-line options and don't like typing things.

### Seatbelt.cna

- Run Seatbelt from the GUI.
- The default settings are:
  - It runs Seatbelt using the `-full` option to return complete results without any filtering. _(Can only be disabled by removing the `-full` string from the code.)_
  - It saves the result to `C:\Windows\Temp\out.txt`. Leaving this option **blank** won't save the result to a file.
- _**Note:** Before using, modify the value of the `$assembly` variable first and point it to the location of the Seatbelt binary._

**Screenshots**

![seatbelt.png](./screenshots/seatbelt.png "Executing Seatbelt")

![seatbelt-command-args.png](./screenshots/seatbelt-command-args.png "Running Command Groups") ![seatbelt-command-groups.png](./screenshots/seatbelt-command-groups.png "Running Command Arguments")

![seatbelt-remote-enum.png](./screenshots/seatbelt-remote-enum.png "Running Remote Enumeration")
---

### SharpHound.cna

- Run SharpHound from the GUI.
- The default settings are:
  - It runs using the `--NoSaveCache` option to prevent writing cache files to disk, which can help with AV and EDR evasion.
  - It saves the result to `C:\Windows\Temp\` directory. Leaving this option **blank** will save the file to the directory where SharpHound was launched from.
- _**Note:** Before using, modify the value of the `$assembly` variable first and point it to the location of the Sharphound binary._

**Screenshots**

![sharphound.png](./screenshots/sharphound.png "Running SharpHound")
