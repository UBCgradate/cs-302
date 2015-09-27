% assignment one 
% Yiming Zhang
% date: 2015/09/15
% show the errors in approximate differentiation of f(x) = sin(x) at x=x0
% plot them at a log-log scale as a function of step size h.
% exact value: fx0=f(x0)=sin(x0),fp1=f'(x0)=cos(x0),fp3f'''(x0) = -cos(x0); 
% approximate expression: (f(x0+h) - f(x0-h))/2h
x0=1.2;
fx0=sin(x0);
fp1=cos(x0);
fp3=-cos(x0);
i=-20:0.5:0;
h=10.^i;
error=abs(fp1-(sin(x0+h)-sin(x0-h))./(2*h));
dis_err=abs(h.^2/6*fp3);
loglog(h,error,'b-*');
hold on
loglog(h,dis_err,'r-.');
legend('Error','Discretization Error')
xlabel('h')
ylabel('Absolute Error')
axis([10^(-20) 1 10^(-15) 1])
