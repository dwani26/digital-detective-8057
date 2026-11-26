# Mission 3 – Understand the Operating System

## 1. Task
In this mission, I explored how an operating system works and what it manages behind the scenes on a computer. I inspected running processes, system storage, file paths, and permissions using the Terminal, while making sure no personal or sensitive details were exposed in my documentation.

---

## 2. Work Completed
Completed Tasks 3.1 to 3.4 in `mission-3-task.md`:
* **Task 3.1:** Checked my macOS version, processor architecture, active user account, disk storage, and running processes via Terminal.
* **Task 3.2:** Learned what processes and Process IDs (PIDs) represent and examined real examples running on my system.
* **Task 3.3:** Practiced using absolute and relative file paths and inspected file access permissions.
* **Task 3.4:** Studied six core responsibilities of an operating system and connected each one to everyday computing examples.


## 3. Commands / Tools Used

`sw_vers`, `uname -m` -  Used these to checked my macOS version and processor architecture details.
`whoami` -  Verified which user account was currently active.
 `df -h /` -  Checked total disk capacity, used storage, and available free space.
`ps aux | head -n 10` - Viewed the first 10 active processes running on my Mac. 
 `pwd`, `cd`, `ls -l` - Checked directory locations, navigated folders, and inspected file permissions.
 Git(`status`, `add`, `commit`, `push`) - Staged, committed, and pushed my Mission 3 work to GitHub.

## 4. What I Understood
I learned that the operating system acts as the bridge that allows hardware and software applications to work together smoothly. It manages critical tasks like running programs, allocating memory, organizing files, and enforcing permissions. I also understood that every active process is assigned a unique **PID** so the OS can track and manage it individually. Before this mission, I hadn't realized how much work the OS handles continuously in the background during normal computer use.

---

## 5. Difficulties Faced
While capturing Terminal outputs and documenting my results, I had to be careful because several command outputs displayed private information such as my Mac username and local folder paths.

---

## 6. How I Fixed Them
I reviewed all command outputs before saving them and replaced private details with `[redacted]` wherever needed. This allowed me to clearly document my work without exposing personal information on GitHub.

---

## 7. Evidence / Files
* `mission-3-task.md` — Contains my detailed answers, command outputs, and observations for Tasks 3.1 to 3.4.
* `README.md` — Provides a structured overview and summary of my work in this mission.

---

## 8. Commit Details
* **Commit Message:** `Document operating system and file management`
* **Push Status:** Committed and pushed the `mission-3` folder to the `main` branch on GitHub.