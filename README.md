Every time you make a new C++ directory, change *launch.json* and *tasks.json* to the files in this repo.

Make sure you have the 'Code Runner' extension installed.
If you are having trouble finding *settings.json*, following these steps:
1. Go into VSCode settings [ (cmd + ,) on Mac ]
2. In the search bar, type 'Code Runner Executor Map'
3. Press 'Edit in settings.json'

***NOTE:*** In my *settings.json* file, the braces on lines 1 and 10 indicates the opening and closing of a json object.
If your *settings.json* file is not empty, do not copy the braces on lines 1 and 10. Add the code from lines 2 to 9 into
your json object.

**ONLY IF YOU ARE RUNNING MacOS M1 Chip**

If you are running on MacOS M1 Chip, add the following line to *launch.json* in configurations:
* "targetArchitecture": "x86_64"

And in *settings.json* add the following code:
*  "cmake.configureArgs": [
        "-DCMAKE_OSX_ARCHITECTURES=x86_64"
    ]
