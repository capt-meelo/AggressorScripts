## AggressorScripts

Collection of scripts that I created to make my life easier since I'm not good at remembering command-line options and don't like typing things.

### CreateTicket.cna

- Generate golden, silver, and trust tickets from the GUI. The created tickets are then injected into the current session.
- The default settings are:
  - It uses the `/endin:600` and `/renewmax:10080` arguments to set the ticket lifetime and the maximum lifetime that a ticket can be renewed.

**Screenshots**

![createticket.png](./screenshots/createticket.png "CreateTicket Menu") 

![createticket-golden.png](./screenshots/createticket-golden.png "Creating Golden Ticket ") 

![createticket-silver.png](./screenshots/createticket-silver.png "Creating Silver Ticket ") 

![createticket-trust.png](./screenshots/createticket-trust.png "Creating Trust Ticket ")
---

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
---