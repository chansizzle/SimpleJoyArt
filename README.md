# SimpleJoyArt
download public domain images

### as of March 8 2024
- [X] script on linux: `simplejoyart-download.sh`
- [ ] script on windows: `simplejoyart-download.ps1`
- [X] 924 images
- [X] 5.2 GB
---


- :blue_book: Running the script will create the directory specified near the top of the script.
- :orange_book: When running each file will display as Downloaded or Failed

![Screenshot from 2024-03-08 14-32-41](https://github.com/chansizzle/SimpleJoyArt/assets/14916599/b1507630-e2b3-4578-a3ca-132e00a000db)

- :notebook: Failed downloads are added to the failures log file specified in the script.
- :closed_book: Failed downloads will be for multiple reasons. There will be many failures for unknown reasons. Legitimate failures are when the URL is no longer valid - renamed, removed, misspelled.
- :notebook_with_decorative_cover: To try downloading the list of failed files again, copy the list of failed downloads from the failures log file and replace the list of URLs in the script with the copied list. Delete the failure log (or rename it) so you do not append the next iteration of failures to the existing list. Then rerun the script.

---
## Using the scripts

### Linux

`download_dir="/DIRECTORY/STRUCTURE/HERE/SimpleJoyArt"`

`download_dir="/home/wom bat/Pictures/SimpleJoyArt"`



### Windows

`$download_dir = "C:\DIRECTORY\STRUCTURE\HERE\SimpleJoyArt"`

`$download_dir = "C:\Users\wom bat\Pictures\SimpleJoyArt"`


```
cd "C:\Users\wom bat\Pictures\SimpleJoyArt"
```


```
PowerShell.exe -ExecutionPolicy Bypass -File .\simplejoyart-download.ps1
```
