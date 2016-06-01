# Gaussian_normal_PDF
%Plotting a Gaussian normal probability density function with N,mean, standard deviation and span given as 500,1.5,0.5 and 10 %respectively in MATLAB

N=500;
u=1.5;
sd=0.5;
span=10;
xmax=u+span/2*sd;
xmin=u-span/2*sd;
x=xmin:((xmax-xmin)/N):xmax;
f=0.3989*exp((-(x-u).^2)/2*sd.^2)/sd;
plot(x,f)
xlabel('x')
ylabel('f(x)')
title('Gaussian Normal PDF')
