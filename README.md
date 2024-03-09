This is a simple program to get the annotations from your Kobo
and export them as a csv file. It should automatically locate 
your Kobo if it is plugged in and shows up in the finder (on Mac).
It shows highlighted text, annotations, date of creation,
author, and book title. You can also specify a specific time range,
author, book, or all three to filter on.

It can be run in the terminal on a mac, I think it also 
will work on Linux, and I don't know about Windows. If it doesn't,
that should only be a problem navigating to the Kobo, which should be an easy fix.

In order to run the file, open the terminal, navigate to file's directory, and write:

```bash
python3 kobo_annotations.py --author "Author Name" --title "Book Title" --start-date YYYY-MM-DD --end-date YYYY-MM-DD --file-name output.csv

```
replacing the arguments with your own, or deleting the ones you don't want to filter on.

All arguments are optional, and if nothing is selected it will make a file with all annotations on the kobo,
creating a file "annotations.csv" in the directory that the file was run in.



____

Used the get_kobo_mountpoint function from Karlikoss's Kobuddy function: https://github.com/karlicoss/kobuddy

