# Python on Windows

Hello!

To install Python, download Python 3.10 (or higher) from http://www.python.org.

Extremely important: when you install it, make sure to check "Add Python to PATH".

Once Python is installed, you can execute the program "cmd.exe ". This is a command-line interface to your computer. Here, just type the word python and that will start the Python program.

At all points during the course, you can always type python name_of_file.py and that will execute the code of a file called name_of_file.py

Multiple versions of Python
If you have multiple versions of Python installed, such as a version you installed a while ago, you can list all of them with this command:

```
py -0p
```

The result will be something like this:

```
C:\Users\youruser>py -0p
Installed Pythons found by py Launcher for Windows
-3.10-64 C:\Users\youruser\AppData\Local\Programs\Python\Python310\python.exe \*
-3.9-64 C:\Users\youruser\AppData\Local\Programs\Python\Python39\python.exe
-3.8-64 C:\Users\youruser\AppData\Local\Programs\Python\Python38\python.exe
-3.7-64 C:\Users\youruser\AppData\Local\Programs\Python\Python37\python.exe
-3.7-32 C:\Program Files (x86)\Python37-32\python.exe
-2.7-64 C:\Python27\python.exe
```

Once you have identified the version you want to use you can run it by doing:

```
py -3.9 file_to_run.py
```

Additionally, if you want to create a new virtual environment with the desired python version, you can do it by running the following command:

```
py -3.9 -m venv name_of_the_venv
```

Finally, if you want more information about the Python launcher for windows, you can check the official documentation:

https://docs.python.org/3/using/windows.html?highlight=launcher#python-launcher-for-windows

Kind regards,

Jose
