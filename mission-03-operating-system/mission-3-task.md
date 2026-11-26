# Mission 3 – Understand the Operating System

## Task 3.1 – Explore Your Operating System

| Information Explored | What It Tells You | What I Observed |
| :--- | :--- | :--- |
| **Operating system / system details** | Shows which OS the computer is running, along with its version and processor architecture. | Confirmed my computer runs macOS using `sw_vers` and checked the chip architecture using `uname -m`. |
| **Current account identity** | Shows which user account is currently logged in. | Checked with `whoami` (username `[redacted]` for privacy) and confirmed I was using a standard local user account rather than the `root` account. |
| **Available and used storage** | Shows how much disk space is used and how much remains free. | Checked the main `/` volume with `df -h /` and viewed the total, used, and available storage in GB. |
| **System activity snapshot** | Shows which programs are running and their CPU and memory usage. | Used `ps aux \| head -n 10` to inspect active processes along with their `%CPU` and `%MEM` usage. |

---

## Task 3.2 – Understand Processes

1. **What is a process?**  
   A process is an active instance of a program currently running on the computer. For example, when I open Google Chrome or VS Code, it launches as a process and consumes system resources like RAM and CPU.

2. **What does the `PID` column represent?**  
   `PID` stands for **Process ID**. The operating system assigns a unique number to every running process so it can track, manage, and stop it individually.

3. **Two examples of processes running on my computer:**
   * **Application process:** Google Chrome or VS Code while actively working.
   * **Background system process:** `WindowServer` or `Finder`, which continuously manage the graphical desktop and on-screen windows.

---

## Task 3.3 – Understand Paths and Permissions

1. **What is the difference between an absolute path and a relative path?**
   * **Absolute path:** Specifies the complete location of a file or folder starting from the root directory (`/`). It works regardless of which folder I am currently in.  
     *Example:* `/Users/[redacted]/Desktop/digital-detective-8432/terminal-practice`
   * **Relative path:** Specifies the location relative to my current working directory, saving me from typing the full path.  
     *Example:* `terminal-practice/notes.txt` (when I am already inside the main assignment folder).

2. **Owner permissions check (`ls -l`):**  
   I checked `terminal-practice/notes.txt` using `ls -l` and observed `-rw-r--r--` as the permission string. This means:
   * **Owner (`rw-`):** I can read and edit the file.
   * **Group & Others (`r--` / `r--`):** Other users can only read the file, and nobody has permission to execute (`x`) it.

---

## Task 3.4 – Explain Operating System Responsibilities

| OS Responsibility | My Explanation | Everyday Example |
| :--- | :--- | :--- |
| **Process management** | Manages active programs and decides how they share CPU time. | Running VS Code, Google Chrome, and Terminal smoothly at the same time. |
| **Memory management** | Tracks and allocates RAM across different running applications. | Assigning RAM to open browser tabs and freeing it when tabs are closed. |
| **Device management** | Enables communication between software and connected hardware devices. | Detecting keyboard keystrokes and trackpad clicks immediately. |
| **File management** | Stores, organizes, and retrieves files and directories on storage drives. | Creating, saving, and renaming my assignment folders in Finder or Terminal. |
| **User interface / shell** | Provides a way for users to interact with the system visually or via text commands. | Navigating via the macOS desktop GUI or typing commands in Terminal. |
| **Security and permissions** | Controls who can access, modify, or execute files and system settings. | Prompting for my password before allowing system-level changes. |