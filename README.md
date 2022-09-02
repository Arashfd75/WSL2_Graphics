# WSL2_Graphics
Showing plots and figures in WSL2

If you have problem showing your plots with WSL2, follow these steps:

1. Download & install [VcXsrv](https://sourceforge.net/projects/vcxsrv/).
2. Run xlaunch.exe (can be found in the installation directory), select multiple windows, tick the disable access control checkbox.
3. Search for Firewall and Network Protection and, in "Allow an app through firewall", manually add VcXsrv.exe and give it both public and private permissions.
4. in WSL2 terminal run: 
>  ``export DISPLAY=`grep -oP "(?<=nameserver ).+" /etc/resolv.conf`:0.0``

