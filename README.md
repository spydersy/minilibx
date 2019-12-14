# minilibx in linux / windows
Minilibx is a very basic graphical library writting in C used in 42
and in Epitech for infography project.
# notes
##update and upgrade ur system:
###apt-get update
###apt-get upgrade
##Install the following packages:
###apt-get install libx11-dev
###apt-get install libxext-dev
##Get minilibx sources:
```
git clone https://github.com/ttshivhula/minilibx minilibx_linux
```
##Add a variable named PKG_CONFIG_PATH containing the path to minilibx_linux directory.
###echo "export PKG_CONFIG_PATH=path_to_minilibx_linux directory" >> ~/.bashrc
##Compile and install mlx.a in minilibx_linux with
###make && sudo make install
##Change MLXFLAGS in your makefile to:
####MLXFLAG = -lm -lmlx -lXext -lX11 -L ./libft -lft -lpthread
###############################################################################
###otherwise you can use ubuntu bash on windows 10 from windows store:
###do the same steps + you have to install gcc and make
###to run graphical Linux programs on your windows 10 desktop
###you need a GUI server, such as X11. Such doesn’t not exist for Windows,
###but there are alternatives, one of which is Xming, which can be downloaded
###free of charge, from SourceForge : https://sourceforge.net/projects/xming/ (set private when ask)
###then enable bash to use xming which can be done by typing the following line
#echo "export DISPLAY=localhost:0.0" >> ~/.bashrc
#its preferable to launch xming automatically after boot, move xming program to the following repo:
#C:\Users\login\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup
-after adding variables such PKG_CONFIG_PATH or DISPLAY, open a new bash session by typing bash
