# Linux Command lines tutorial

This tutorial aim to introduce basic but popular command lines in Linux terminal.

You can refer the my the YouTube playlist(expained in khmer) [here](https://www.youtube.com/playlist?list=PLR9cB9dCWlxfLwaLnmz8c34XMxxT7T11A).

## Tutorial 1

1.  `ctr+alt+t`: open the terminal
2.  `~`: home or user or personal directory
3.  `l`, `ls`, `la`: list the files or folder in the current directory
4.  `cd` : change directory
    - `cd folderName`: move to 'folderName' in the working directory
    - `cd ..`: move to the parent directory
    - `cd .` : move to the same directory
    - `cd ~` or `cd` : move to the home directory
5.  `pwd`: print working directory
6.  `mkdir`: make directory
7.  `rmdir`: remove directory(only if it is an empty folder)

## Tutorial 2

8. `touch fileName` : create an empty file named 'fileName'
9. `rm fileName`: remove the 'fileName' file
10. `rm -r folderName`: remove recurcively all the files and folders in 'folderName' folder
11. `cp fileName targetFolder`: copy the 'fileName' file to the 'targetFolder' directory
12. `cp -r folderName targetFolder`: copy the 'folderName' folder to the 'targetFolder' folder
13. `mv source targetFolder`: move 'source' file or folder to the 'targetFolder' directory
14. `tree`: list contents of directories in a tree-like format
15. Special symbols and charactors:
    - `/`: seperate the path of the folder and file or subfolders (It represents also the root directory.)
    - `~`: shortcut to the personal directory
    - `.`: the current directory
    - `..`: the parent directory of the current directory
    - `*`: replace infinite of characters(or even nothing)
    - `?`: replace one and only one character.

# Tutorial 3

16. `history` : priview the last 1000 commands
17. Tricky key binding

    - `up/down arrow key`: move to the previous or next command
    - `tab`: autocompletion
    - `ctr+r`: search the history that match what you type
    - `ctr+u`: delete everything on the left-hand side of the curser
    - `ctr+k`: delete everything on the right-hand side of the curser
    - `ctr+shift+t`:open new tab
    - `ctr+pageUp/pageDown`: switch to
    - `-h` or `--help`: display the usage document for a command
    - `alt+i`: move to the $i^{th}$ tab in the terminal
      - _ex_ :`alt+2`: move to the second tab

18. funny and cool commands

    - `cmatrix`
    - `cal`
    - `say`
