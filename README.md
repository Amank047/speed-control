# Function block code
function [R,Y,B] = fcn(time,freq)
omega=2*pi*freq;
R=sin(omega*time)*freq/60;
B=sin(omega*time+120*pi/180)*freq/60;
Y=sin(omega*time+240*pi/180)*freq/60;
