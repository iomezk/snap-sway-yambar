# Sway WM with Yambar panel
\
This snap requires access to the system logind. (as a root user):  
`snap connect sway-yambar:login-session-control`  
`snap connect sway-yambar:login-session-observe`

Also to fix Firefox crashes it's currently needed:  
`snap connect firefox:wayland sway-yambar`

Then start Sway in a free tty as a non-privileged user:  
`exec sway-yambar`

HOME directory of this snap is /home/$USER/snap/sway-yambar/common/  
Default configs can be obtained from /snap/sway-yambar/current/etc/  
Launching a `foot-terminal` snap using $mod+Enter hotkey is supported out of the box.
