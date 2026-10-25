---
name: mikrotik-winbox-connect
description: "Open WinBox and connect to a MikroTik router using the correct address and credentials."
allowed-tools:
  - Glob
  - Bash(*)
---

---
name: mikrotik-winbox-connect
description: Open WinBox and connect to a MikroTik router using the correct address and credentials.
allowed-tools:
  - Glob
  - Bash(*)
---

When to use: Use this skill when you need to open the WinBox client and establish a connection to a MikroTik router from the local machine.

1. Locate WinBox.
   Find the installed WinBox executable on the local machine. If it is missing, obtain the official MikroTik client and note the exact path before launching it.
   Use `glob` to search common install locations, then confirm the final path with `bash` if needed.

2. Launch the client.
   Start WinBox from the located executable and wait for the login window or connection dialog to become available.
   Use `bash` to launch the executable and keep the process open until the UI is ready.

3. Connect to the router.
   Use the MikroTik router's address or hostname and the correct admin credentials to open a WinBox session to the target device.
   Use `bash` to provide the connection details in the WinBox application and authenticate with the administrator account.

Edge cases:
- If the executable is not found, install the official MikroTik WinBox client from the vendor source before proceeding.
- If the router address is not known, confirm the correct IP address or hostname from your network settings or the target environment.
- If authentication fails, verify the admin credentials and ensure the router is reachable from the local machine before retrying.
