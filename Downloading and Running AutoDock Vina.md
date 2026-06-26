</> markdown
## Downloading AutoDock Vina
- Type download autodock vina for windows 11 in the URL or address bar of a browser window. 
- Select the first link: https://vina.scripps.edu/downloads/ or AutoDock Vina Downloads.
- Under Download click on Source code (GitHub), https://github.com/ccsb-scripps
- In pinned or repositories click on AutoDock Vina Public: https://github.com/ccsb-scripps/AutoDock-Vina
- On page AutoDock Vina Public on the right hand side under releases click on latest v1.2.7 
- You will reach this URL: https://github.com/ccsb-scripps/AutoDock-Vina/releases/tag/v1.2.7
- For windows from the asset list select: 
  -- vina_1.2.7_win.exe (1.18 Mb)
  -- vina_split_1.2.7_win.exe (672 KB)
- Download the above two into a folder created in the C drive called Vina.

 ## RUNNING AutoDock Vina from Command Line
- Running Vina requires receptor.pbdqt, ligand.pdbqt, and config.txt files in the folder with AutoDock Vina.exe files  (downloaded in the last step). 
- The receptor and ligand .pdbqt files are prepared using AutoDock Tools (ADT) v1.5.7 (Discussed Elsewhere).
- The config.txt files will be created using notepad in windows (Discussed Elsewhere). 
- Open the command line using the Windows key plus R keys, opening a window called Run with cmd, click OK.
- The new window with the should have the following command prompt: C:\Users\Admin>
- Type cd /d C:\Vina\DOCKING\MMP1 and press enter, where cd means change director and /d means change drive also if you want to change drive, followed by full path of the folder where you want to go
- If you see C:\Vina\DOCKING\MMP1 it means you have reached the docking directory.
- For checking files in the directory, type dir and press enter
- You should be able to see all the files i.e. .pdbqt, .txt, and .exe
- At prompt type vina_1.2.7_win.exe
- You should be see all specifications of vina
- At prompt now type vina_1.2.7_win.exe –config config.txt --out docked.pdbqt and press enter
- This will run Vina and output will contain binding affinity values and rmsd values.
- Also the MMP1 folder in Vina should now contained docked.pdbqt file, which can be opened in ChimeraX v1.11.1 or Chimera v1.19 under tools and view dock.


