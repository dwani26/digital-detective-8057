# Mission 2: Become Comfortable with the Terminal

## Task 2.1 – Explore Basic Terminal Operations

| Command | What It Does | What I Observed |
| :--- | :--- | :--- |
| `pwd` | Shows the folder I am currently in. | Displayed the full path to my repository folder. |
| `ls` | Lists the files and folders in the current directory. | Showed all my mission folders along with the `README` file. |
| `ls -l` | Lists files with extra details like size and permissions. | Displayed each file and folder on a separate line with metadata. |
| `cd ..` | Moves one directory level back (to the parent folder). | Running `pwd` afterward confirmed I had moved to the parent folder. |
| `mkdir` | Creates a new folder. | Created my new practice directory cleanly. |
| `touch` | Creates a new empty file. | Generated a blank text file with 0 bytes. |
| `cp` | Copies a file to a specified name or path. | Both the original file and the duplicated copy appeared in the folder. |
| `mv` | Moves or renames a file. | Updated the old filename directly to the new one. |
| `cat` | Displays the contents of a file. | Printed the file's text directly inside the Terminal window. |

---

## Task 2.2 – Practise File Changes Safely

1. **What is the difference between replacing a file's contents and adding text to the end?**  
   Using `>` overwrites the file, replacing all existing content with the new text. Using `>>` appends the new text to the end of the file while keeping the original content intact.

2. **What is the difference between copying a file and moving a file?**  
   `cp` creates an exact duplicate of the file, leaving the original untouched in its place. `mv` relocates the file to a different directory or renames it without leaving a duplicate behind.

3. **What information does the current directory display provide?**  
   The `pwd` (Print Working Directory) command shows the exact folder path I am currently working in. This helps verify my location so I don't accidentally create, modify, or delete files in the wrong place.

4. **Why is a directory-listing operation useful?**  
   Commands like `ls` let me quickly see all visible files and subfolders in my current location. Adding flags like `ls -l` shows extra details (such as permissions and timestamps), making it easy to verify that files were created, moved, or renamed properly.

---

## Task 2.3 – Understand Flags and Pipes

1. **Normal listing (`ls`) vs. detailed listing (`ls -lah`)**  
   * `ls` displays only the names of visible files and folders.  
   * `ls -lah` provides a complete breakdown: `-l` shows detailed metadata (permissions, ownership, dates), `-a` reveals hidden files like `.git`, and `-h` formats file sizes into human-readable units (KB, MB).

2. **Pipe example (`ls -l | head -n 5`) and how it works**  
   The `|` symbol (pipe) takes the standard output of the first command and passes it directly as input to the next command:
   * `ls -l` generates the full detailed list of files and folders.
   * `head -n 5` filters that output to display only the first 5 lines, keeping the Terminal output clean and concise.

---

## Task 2.4 – Understand Package Managers

A package manager automates installing, updating, configuring, and removing software directly from the Terminal, eliminating the need to manually download installers from websites. 

* **Example (macOS):** **Homebrew** (`brew`), which lets developers quickly install command-line tools, libraries, and applications using simple commands like `brew install <package>`.