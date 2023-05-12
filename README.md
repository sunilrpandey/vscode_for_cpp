# VS Code setup for C++ on Windows
## <a name = basics> What is required </a>

Since visual studio code is just a source code editor for multiple language including C++. We need below things to setup a good C++ dev environment.

- [ ] Install VS Code for windows
- [ ] C++ specific formatter which helps while we write code. VS code provides various extensions to help in this such as C/C++ Extensions by Microsoft
- [ ] C++ Compiler(such as mingw) to be used for code compilation

Now we have editor and compiler, let us write our code, compile, debug and run.

##  Write Code
VS Code provides various extensions to help with intelligence, indentation, static analysis, formatting etc. 

You can open visual studio code extension using [ctrl + shift + x] or View->Extensions. 
Just for begining, Search for C/C++ extension from Microsoft and install it from vs code itself.

Go to Command Pallete (Ctrl + Shift + P) and select C/C++: Edit Configurations to Add dependent includePath and library path in C_CPP_Properties.json

##  Build Code
Go to Command Pallete (Ctrl + Shift + P) and select Task: Configure Task to create/modify task.json to configure compiler path, command etc

##  Launch Code - Debug/Run
Go to Run and Debug in left side bar (Ctrl + Shift + D) and configure program to run and other dependencies by editing launch.json 

### Please note above build/launch would be created for selected file only therefore make sure .cpp is selected. Also you can compile/run the code using  g++ compilation command such as g++ -g <cpp file name> -o <output file name> and run from command line

### <a name = vs_install>Install VSCode on Windows</a>
Go to [VS Code download page](https://code.visualstudio.com/download) and download vscode for Windows and install by double clicking the downloaded installer and following installation steps. 

### <a name = compiler_install>Install C++ Compiler - MINGW</a>

Please do check if MINGW is already installed on your system. Dont look it in \'Program Files\' folder since generally MINGW is installed using copy/paste way and it is copied in C:\MINGW or similar. Even if it is installed using installer it copies at C:\MINGW only. You can also check environment path where it might have been added if it was installed earlier

Go to [MINGW download page](https://sourceforge.net/projects/mingw-w64/files/latest/download) and download vscode for Windows and install by double clicking the downloaded installer and following installation steps. which will copy mingw installation files at C:\MINGW or C:\MINGW64. Add it to PATH by editing environment variables.



- [ ] [Keyboard shortcuts ](#shortkey)
- [ ] [Extensions](#ext)
- [ ] [Misc](#ext)


## <a name = misc>Misc</a>
**Ctrl + M  : Toggle Use of Tab Key for Setting Focus/and entring space**


## <a name = shortkey>keyboard Shortcuts</a>
- Copy path of active file : Ctrl+K P 
- Reveal active file in File Explorer : Ctrl+K R 
- Show active file in new window/instance : Ctrl+K O 

- Show preview for markdown : Ctrl + K, V
- Show hover : Ctrl+K Ctrl+I 
- Toggle Panel(Terminal etc) : Ctrl + J
- Toggle Sidebar(Explorer bar etc) : Ctrl + B
- Explorer Bar : ctrl + shift + E
- Select Color Theme : Ctrl K + Ctrl T

- Extension explorer : ctrl + shift + x
- Preference(command palette) : ctrl + shift + p
- Keyboard Binding : Ctrl + k + s
- Open/Goto file : ctrl + p

- Select current line : Ctrl+L 
- Line up/Down : ALt + Up/Down
- Delete Line : Ctrl + shift + k
- Go to Line number : Ctrl+G 
- Select all occurrences of current selection : Ctrl+Shift+L 

- Go to Definition : F12 
- Peek Definition : Alt+F12 
- Open Definition to the side : Ctrl+K F12 
- Show References : Shift+F12 
- Run  - Ctrl + Shift + D

- Go back / forward : Alt+ ← / → 
- Select all occurences of Find match : Alt+Enter 
- Select all occurrences of current word : Ctrl+F2 
- Toggle case-sensitive / regex / whole word : Alt+C / R / W
- Insert line below : Ctrl+Enter 
- Insert line above : Ctrl+Shift+Enter 
- Scroll page up/down : Alt+PgUp / PgDn 
- Add line comment : Ctrl+K Ctrl+C 
- Remove line comment : Ctrl+K Ctrl+U 

- Trigger suggestion : Ctrl+Space 
- Trigger parameter hints : Ctrl+Shift+Space 
- Format document : Shift+Alt+F 
- Format selection : Ctrl+K Ctrl+F 
- Quick Fix : Ctrl+. 
- Toggle word wrap : Alt+Z 


- Focus into 1st, 2nd or 3rd editor group : Ctrl+ 1 / 2 / 3 

## <a name = ext>VSCode Extensions</a>
- Python, C/C++, Docker by Microsoft
- GitLens by EricAmodio
- Zuul Job Browser
- Pylance by Microsoft
