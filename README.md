# Back2Phase2

B2P2: Back2Phase2 Launcher
B2P2 is a specialized version-management utility for Project: Playtime, developed entirely in Python. It allows users to download, manage, and switch between Phase 2 (Incineration) and Phase 3 (Destroy-a-Toy) using high-speed direct downloads.

Key Features
Python-Powered Logic: Built with Python for efficient file handling and system-level automation.

Direct Download Integration: Fetches Phase 2 assets directly from high-capacity storage servers to ensure a smooth setup.

Visual Progress Bar: Real-time tracking of download progress and completion percentages within the terminal.

Zero-Latency Switching: Uses folder-renaming logic to swap game versions in under a second.

Smart State Detection: Automatically identifies the active version via is_phase2.txt or is_phase3.txt markers.

Automated Backups: Safely renames your existing game folder before applying the swap to prevent data loss.

Requirements
Windows 10 or 11.

Administrator Privileges: Required for modifying the Program Files (x86) directory and hooking keyboard inputs.

Stable Internet Connection: Required for the initial download of Phase 2 assets.

Project: Playtime (Steam): The game must already be installed in your Steam library.

Installation
For Users (EXE)
Download the B2P2.exe executable.

Place the EXE in its own dedicated folder (e.g., C:\B2P2).

Right-click the file and select Run as Administrator.

Select "Install Phase 2 Files" to begin the automated download and extraction.

For Developers (Python Source)
To run the script from source, ensure you have Python 3.x installed along with the following libraries:

Bash
pip install requests keyboard colorama
Run the script using:

Bash
python main.py
Instructions
Navigation: Use the UP and DOWN arrow keys to move the highlight in the menu.

Selection: Press ENTER to confirm your selection.

The Swap Process:

Switch to Phase 2: Renames the "Poppy Playtime - Multiplayer" folder to "..._Phase 3" and activates your Phase 2 folder.

Switch to Phase 3: Reverts the folders back to the standard Steam version.

Auto-Launch: Once the swap is successfully completed, B2P2 will automatically trigger Steam to launch the game.

Troubleshooting
Permission Denied: You must run the program as Administrator. Windows security prevents unauthorized scripts from modifying the Steam directory.

Download Interruptions: Ensure you have at least 15GB of free disk space to accommodate both the compressed archive and the extracted game files.

Game Verification: If Steam reports missing files after a swap, use B2P2 to switch back to Phase 3 and use the "Verify Integrity of Game Files" feature within Steam before attempting the swap again.

Credits
Lead Developer: NotCotik

Language: Python 3.x

Interface: B2P2 Stylized CLI
