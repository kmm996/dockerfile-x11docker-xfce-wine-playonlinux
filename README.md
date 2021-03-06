# x11docker/xfce-wine-playonlinux

XFCE desktop containing wine, pulseaudio, winetricks, q4wine and playonlinux

 - Use x11docker to run image on a second X server with GUI and pulseaudio sound support. 
 - Get x11docker and x11docker-gui from github: 
https://github.com/mviereck/x11docker 

# Examples:
 - Run XFCE desktop including wine and playonlinux on separate, new X server:
  - `x11docker --desktop x11docker/xfce-wine-playonlinux`

 - Use host folder to preserve installed Windows applications. Create a container user similar to your host user to avoid file permission issues:
  - `x11docker --desktop --hostuser --home x11docker/xfce-wine-playonlinux start`

- Use host folder to preserve installed Windows applications. Create a container user similar to your host user to avoid file permission issues. Show xfce-wine-playonlinux in a window on your main desktop:
 - `x11docker --xephyr --desktop --hostuser --home x11docker/xfce-wine-playonlinux start`

- Use host folder to preserve installed Windows applications. Create a container user similar to your host user to avoid file permission issues. Show PlayOnLinux in a window on your main desktop:
 - `x11docker --xpra --hostuser --home x11docker/xfce-wine-playonlinux playonlinux`
 
 # Screenshot
 Screenshot showing xfce desktop with wine and pulseaudio enabled in a Xephyr window, using [x11docker](https://github.com/mviereck/x11docker), with shared home folder to preserve wine installations and desktop settings.
 
 ![screenshot](https://raw.githubusercontent.com/mviereck/x11docker/screenshots/screenshot-xfce-wine-playonlinux.png "xfce-wine-playonlinux desktop running in Xephyr window using x11docker")

