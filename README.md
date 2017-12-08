# FontAwesome 4 to 5
**A small Python tool to convert icons in files from FontAwesome 4 to 5**  
**This may be unstable. We strongly suggest a full backup before proceed.**

FontAwesome 4 to 5 is brought to you by Giovdi by Pixelstyle.it.

A FontAwesome 3 to 4 converter is also available at [https://github.com/giovdi/fontawesome-3-to-4](https://github.com/giovdi/fontawesome-3-to-4)

## Notes

* **This converter works only if the `fa` class is IMMEDIATELY followed by an icon class (e.g. `fa fa-ok`).**  
* All modifiers (`fa-spin`, `fa-fw`, `fa-li`...) will be notified for manual review.
* The icons replaced are based on the official list on fontawesome.com: [Upgrading from Version 4](https://fontawesome.com/how-to-use/upgrading-from-4#icon-name-changes).

## How to use it
In `main.py` you can define the file or the folders you want to check.  
Use `pathCheck` to check every file into a folder or `fileCheck` to check a single file.

For example:
```
# For Windows users
FontAwesome4to5.pathCheck("C:/path/to/folder", True)
FontAwesome4to5.fileCheck("C:/path/to/file.php", True)
# For Unix users
FontAwesome4to5.pathCheck("/path/to/folder", True)
FontAwesome4to5.fileCheck("/path/to/file.php", True)
```

The first parameter is a folder or a file to convert, the second one, if True, creates a .bak file for each file analyzed.

To quickly use this tool, feel free to change `main.py` with your paths and files.  
You can also use `from fontawesome4to5 import FontAwesome4to5` to use this library in your projects.

## Eclipse integration
You can import this project into your Eclipse workspace to easly use the library standalone.

## Requirements
The script uses Python 2.7 to work