# ArchLinux_Nvidia_PrimeScreen

This workaround is  Deprecated use the below instructions instead  


**Use this method instead**
if you have a hybrid gpu as intel and nvidia and if you want to use nvidia gpu for screens
on arch linux then use 
the system76-power service 
https://aur.archlinux.org/packages/system76-power/
no need to modify any files anymore
install the system76-power service from the above aur repo using yay ( yet another yarourt )
then  enable the system76-power.service using ```sudo systemctl enable system76-power.service```
after that you can use the hybrid/nvidia only preference using 

#hybrid
```sudo system76-power graphics hybrid``` 

**reboot**
this will enable the intel gpu to be used for display and nvidia gpu for graphics intensive task (games)

#nvidia only
```sudo system76-power graphics  nvidia```

**reboot**

this will enable the nvidia gpu to be used for both display and gpu intensive tasks
(note :- i use this mode as my intel 630 doesn't provide a smooth UI experience on gnome) 