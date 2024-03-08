# SimpleJoyArt
download public domain images

### as of March 8 2024
- [X] script on linux: `simplejoyart-download.sh`
- [ ] script on windows: not created yet
- [X] 924 images
- [X] 5.1GB
---


- :blue_book: Running the script will create the directory specified near the top of the script.
- :orange_book: When running each file will display as Dowbnloaded or Failed

![Screenshot from 2024-03-08 14-32-41](https://github.com/chansizzle/SimpleJoyArt/assets/14916599/b1507630-e2b3-4578-a3ca-132e00a000db)

- :notebook: Failed downloads are added to the failures log file specified in the script.
- :closed_book: Failed downloads will be for multiple reasons. Usually the URL is no longer valid - renamed, removed, misspelled.
- :notebook_with_decorative_cover: To try downloading the list of failed files again, copy the list of failed downloads from the failures log file and replace the list of URLs in the script with the copied list. Then rerun the script.