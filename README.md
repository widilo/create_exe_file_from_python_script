# How to Create a Windows Executable from a Python Script

Turning your Python script into a standalone .exe file is simple with PyInstaller. Follow this guide to generate an executable that can run on Windows without requiring Python installation.

### 1. Install PyInstaller

First, install PyInstaller if you haven’t already:

```bash
pip install pyinstaller
```

### 2. Convert the Script to an Executable

Run the following command in the terminal or command prompt:

```bash
pyinstaller --onefile --windowed yourscript.py
```

Explanation of Flags:

```bash
    --onefile: Creates a single executable instead of multiple files.
    --windowed (optional): Hides the console window (useful for GUI applications). Omit this flag for CLI scripts.
```

### 3. Find the Executable

After running the command, PyInstaller will generate files in the dist folder. Your `.exe` will be located at:

```bash
dist/yourscript.exe
```

### 4. Running the Executable

Navigate to the dist folder and run:

```bash
yourscript.exe
```

### 5. (Optional) Add an Icon

If you want to add a custom icon, use:

```bash
pyinstaller --onefile --icon=icon.ico yourscript.py
```

Make sure `icon.ico` is in the same directory as your script.

## License

<p xmlns:cc="http://creativecommons.org/ns#"  xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title"  rel="cc:attributionURL"  href="https://github.com/widilo/compare-two-excel-files-with-python">Compare two Excel files using Python</a> by <a rel="cc:attributionURL dct:creator"  property="cc:attributionName"  href="https://widilo.de">widilo</a> is licensed under  <a  href="http://creativecommons.org/licenses/by-nc-sa/4.0/?ref=chooser-v1"  target="_blank" rel="license noopener noreferrer"  style="display:inline-block;">CC BY-NC-SA 4.0 <br><br><img  style="height:22px!important;margin-left:3px;vertical-align:text-bottom;"   src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img   style="height:22px!important;margin-left:3px;vertical-align:text-bottom;"   src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img   style="height:22px!important;margin-left:3px;vertical-align:text-bottom;"   src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"><img   style="height:22px!important;margin-left:3px;vertical-align:text-bottom;"   src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1"></a></p> 
