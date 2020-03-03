# **Simulador de Fisica**
Simulador de física para ondas electromagnéticas en Matlab.

## **Simulador 1**
Simulador de ondas electromagnéticas, en proceso de un plano en tres dimensiones.

```matlab

E = 2;
H = 3;
t = linspace(0, 2*pi);
omega = 2;
k = pi/2;
x = ones(size(t));
c = cos(omega*t - k*x);
figure
patch([t fliplr(t)], [c zeros(size(c))], [zeros(size(t)) zeros(size(t))], 'b')
hold on
patch([t fliplr(t)], [zeros(size(t)) zeros(size(t))], [c zeros(size(c))], 'r')
hold off
grid on
view(40, 40)

```

![alt text](Oscilaciones.PNG)