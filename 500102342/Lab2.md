Lab 2:

# Installing WSL (Windows Subsystem for Linux) on Windows

The Windows Subsystem for Linux (WSL) provides a robust and efficient way to run a Linux environment directly on Windows without the overhead of a virtual machine. This guide outlines a professional and streamlined approach to installing WSL on your Windows system.

---

## Step 1: Enable WSL

1. **Open PowerShell as Administrator:**
   - Right-click on the *Start* button and select *Windows Terminal (Admin)* or *PowerShell (Admin)*.

2. **Install WSL:**
   - Run the following command to enable WSL and install the default Linux distribution (typically Ubuntu):
   ```sh
   wsl --install
   ```

3. **Restart Your Computer:**
   - A system reboot may be required to complete the installation process.

---

## Step 2: Verify the WSL Installation

To verify which version of WSL is installed, execute the following command:
```sh
wsl --list --verbose
```

If WSL 2 is not installed, update it using:
```sh
wsl --update
```

---

## Step 3: Install a Linux Distribution

1. **List Available Distributions:**
   ```sh
   wsl --list --online
   ```

2. **Install Your Preferred Distribution:**
   For example, to install *Ubuntu*, execute:
   ```sh
   wsl --install -d Ubuntu
   ```

3. **Set Up the Linux Environment:**
   Launch *Ubuntu* (or your chosen distribution) from the Start menu and follow the setup prompts to create a username and password.

---

## Step 4: Configure WSL Version to WSL 2

Set WSL 2 as the default version by running:
```sh
wsl --set-default-version 2
```

To apply WSL 2 to a specific distribution:
```sh
wsl --set-version Ubuntu 2
```

---

## Step 5: Update the WSL Kernel (Optional)

If prompted to update WSL 2, download and install the latest kernel update from Microsoft:
[Download WSL Kernel Update](https://aka.ms/wsl2kernel)

---

## Step 6: Execute Linux Commands in WSL

You can now run Linux commands through:
- The *WSL terminal* (e.g., Ubuntu or other distributions)
- *Windows Terminal*
- *PowerShell* or *Command Prompt*, using the `wsl` prefix:
```sh
wsl ls -la
```

---

## Step 7: Access Windows Files from WSL

Access your Windows files from the WSL terminal using the `/mnt/c/` directory:
```sh
cd /mnt/c/Users/YourUsername
ls
```

---

## Step 8: Uninstalling WSL (Optional)

To completely remove WSL from your system, follow these steps:

1. **Remove Linux Distributions:**
   - Navigate to *Settings > Apps* and uninstall the Linux distributions.

2. **Unregister WSL Distributions:**
   ```sh
   wsl --unregister <DistroName>
   ```

3. **Disable WSL Feature:**
   ```sh
   dism.exe /online /disable-feature /featurename:Microsoft-Windows-Subsystem-Linux /norestart
   ```

4. **Restart Your System** to finalize the changes.

---

