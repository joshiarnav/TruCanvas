# Building Software

Welcome to the TruCanvas build instructions!

Building and running TruCanvas is very easy due to the use of the "Dub" package manager. The only prerequisites are to confirm that a compiler for D (such as DMD) and SDL are installed!

DLang compilers can be found [here](https://dlang.org/download.html) and instructions to install SDL2 can be found [here](https://wiki.libsdl.org/SDL2/Installation).

Finally, all that is left is to navigate to the `./FinalProject` folder within the root directory and run the command `dub run`! Dub should handle confirming that all dependencies are working appropriately. If you are not familiar with the commands and have this project open in something such as VSCode (meaning that your terminal will already be in the root directory - if not, navigate here using the `cd` command), you can press (in the app bar at the top of VSCode): `Terminal` -> `New Terminal`. Then, in the terminal that pops up, issue the following commands:

```
cd FinalProject/
dub run
```

or

```
cd FinalProject/ && dub run
```

Now the app should be running and you should have the choice to create either a server or a client. If this is the first thread/terminal you are running and you wish to host the server (required for any clients to join) then type `0` and press enter/return. If you already have the server running or it is running elsewhere, press `1` at this step. Then, copy in the section of the "server IP" (in the terminal after starting the server) before the colon (":") into the host and type the section after the colon into the port (i.e. if the IP was `123.456.789:1234`, then the host would be `123.456.789` and the port would be `1234`). And that's all there is to it! Have fun drawing live with your friends!

Note: This project has been tested primarily on macOS and Windows, but should run on all operating systems supported by Dlang and SDL2.
