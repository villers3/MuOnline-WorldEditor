## MuOnline-WorldEditor  
[![WorldEditor](https://img.youtube.com/vi/629J5BmGAXQ/hqdefault.jpg)](https://youtu.be/629J5BmGAXQ)  
  
This is an in-game WorldEditor for Mu Online Season 16e1 (Main version : 1.19.46)  
(No support for other versions)  
Main 1.19.46 unpacked by me can be found here: "https://github.com/VD1988/MuOnline_S16_Lgd/tree/main/Main"  
  
It's been testing with server files released by MuLegend.  
For server installation helps, please visit "https://forum.ragezone.com/f197/release-legend-mu-client-amp-1195391/".  
  
Beside the server, you also need to add codes to load the WorldEditor dynamic library into client's Main.dll source (also released by MuLegend).  
Copy these lines to Main.cpp :  
```
	HINSTANCE hInstance = LoadLibraryA("Plugins\\WorldEditor.dll");
	if (!hInstance) 
		MessageBoxA(NULL, "Could not load the WorldEditor.dll", "ERROR", MB_OK);
```
Or hooking directly from main.exe is also OK.  
Then remember to copy-paste "Plugins" folder to the client location.  
```
//  MuOnline-Client
//  |- main.exe
//  |- Main.dll
//  |--Plugins
//    |-WorldEditor.dll
//    |-Config.ini
//    ...
//
```

# This project is incompleted.
