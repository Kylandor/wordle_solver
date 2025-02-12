# === Squabble Bot ===

## Prerequisites

You need to install the following packages in order to make the program work:

```
pip install keyboard
pip install pyautogui
pip install pillow
```

## How to Use

If you are using this on windows, running any of this code on WSL will NOT work. Use powershell instead.

1. Open a powershell in the folder that has all the code

2. run 

   ```bash
   python .\solver.py
   ```

3. You should see "reset Grid?" pop up. If you are running this for the first time read the next steps so you can understand what to do. It is recommended that you press 'y' in order for the program to recognize where should it look for the squabble grid on screen, but do not press 'y' just yet

4. In order to get an accurate grid position, you need to start a squabble game somewhere on your computer. When the grid is visible, go back to the powershell, press 'y' then enter. The program will take a screenshot and then it will look for the grid. If everything worked properly, you should see a "GRID FOUND" message along with 3 values: startx, endy, and next. Go ahead and copy these values in solver.py line 101

5. To check whether the grid was found correctly, go into the folder that contains all the code and look for a "grid.png". This will show you the screenshot with some red dots of where the program thinks the grid is. It should look something like this:![grid2](C:\Users\ivartic\Desktop\ilieMAKE_BackUp\squable\wordle_solver\grid2.png)

6. If the dots are inside the boxes you should be good and everything else should work correctly

7. Now the powershell will say: "Would you like to play Squabble?". Press 'y' then enter

8. If you want the bot to play for you press 'y' then enter and then very quickly click on the browser that is running squabble. Now the bot should be taking care of the rest. If any problems arise, leave it as an issue in the github

9. When the game is over, the program should crash 

10. Sometimes the bot may enter words that are not accepted, do not worry, the bot will remove that word and try with another guess