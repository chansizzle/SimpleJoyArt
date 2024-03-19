# SimpleJoyArt
download public domain images from the Simple Joy Art spreadsheet

### as of March 8 2024
- [X] script on linux: `simplejoyart-download.sh`
- [X] script on windows: `simplejoyart-download.ps1`
- [X] 924 images
- [X] 5.2 GB
---


- :blue_book: Running the script will create the directory, specified near the top of the script.
- :orange_book: When running each file will display as Downloaded or Failed
- :notebook: Failed downloads are added to the failures log file, specified near the top of the script.
- :closed_book: Failed downloads will be for multiple reasons. There will be many failures with unknown causes. Legitimate failures are when the URL is no longer valid - renamed, removed, misspelled.
- :notebook_with_decorative_cover: Try downloading the list of failed files again. To do so,
  1. copy the list of failed downloads from the failures log file
  2. replace the list of URLs in the script with the copied list
  3. delete the failure log (or rename it) so you do not append the next iteration of failures to the existing list
  4. rerun the script

### Linux
(multiple successes, 1 failure)
![Screenshot from 2024-03-08 14-32-41](https://github.com/chansizzle/SimpleJoyArt/assets/14916599/b1507630-e2b3-4578-a3ca-132e00a000db)


### Windows
(multiple successes, 1 failure)
![Screenshot 2024-03-11 120802](https://github.com/chansizzle/SimpleJoyArt/assets/14916599/545b72bc-5048-45f3-8e39-00d3e1ebba76)

---
## Using the scripts

### Linux

1. download `simplejoyart-download.sh`
2. (from command line) change to the directory where you have saved the script example `cd /home/fancy/scripts`
3. edit the script by changing `download_dir="/DIRECTORY/STRUCTURE/HERE/SimpleJoyArt"` to your desired location. example: `download_dir="/home/wom bat/Pictures/SimpleJoyArt"`
4. save and close the script
5. make the script executable
```
chmod +x simplejoyart-download.sh
```
6. execute the script
```
./simplejoyart-download.sh
```

The `SimpleJoyArt` directory is created and the images are downloaded into this directory.
Some files fail to download for unknown reasons. It is possible for some links to image files to no longer be valid. This type of failure will always fail as the link is not a valid link. As you end up with repeatedly failures, manually check some of the URLs to see if they still work by copying the image link and pasting it into a web browser.

7. Open the failures log file within the SimpleJoyArt directory (the name is specified in the script)
8. Copy the contents of the failures log file
9. edit the script by replacing **all** of the image links with the contents copied from the failures log file.
10. save and close the script
11. delete the failures log file
12. run the script again
13. repeat steps 7-12 until all files have downloaded
 


---
### Windows

1. download `simplejoyart-download.ps1`
2. edit the script by changing `$download_dir = "C:\DIRECTORY\STRUCTURE\HERE\SimpleJoyArt"` to your desired location. example: `$download_dir = "C:\Users\wom bat\Pictures\SimpleJoyArt"`
4. save and close the script
5. open Powershell from the start menu (press the start button and start typing the name. when you see Powershell, right-click on it and select **Run as Administrator**)
6. (from powershell command line) change to the directory where you have saved the script. example `cd "C:\Users\wom bat\scripts"` (enclosing the directory structure in quotes is required if there are any spaces in the directory string)
7. run the script
```
PowerShell.exe -ExecutionPolicy Bypass -File .\simplejoyart-download.ps1
```

The `SimpleJoyArt` directory is created and the images are downloaded into this directory.
Some files fail to download for unknown reasons. It is possible for some links to image files to no longer be valid. This type of failure will always fail as the link is not a valid link. As you end up with repeatedly failures, manually check some of the URLs to see if they still work by copying the image link and pasting it into a web browser.

8. Open the failures log file within the SimpleJoyArt directory (the name is specified in the script)
9. Copy the contents of the failures log file
10. edit the script by replacing **all** of the image links with the contents copied from the failures log file.
11. save and close the script
12. delete the failures log file
13. run the script again
14. repeat steps 7-12 until all files have downloaded
