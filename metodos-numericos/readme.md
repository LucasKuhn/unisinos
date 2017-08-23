# loop for ( -.- )

### Para fazer o vetor:  
           1
           8
          27
          64
         125
         216
         343
         512
         729
        1000

for i=1:10  
v(i)=i^3;  
 end  
 v'  # Apostrofe só pra printar em forma de coluna -.-

### Para a matriz Aij=2i+j
A =

     3     4     5
     5     6     7

for i=1:2  
for j=1:3  
A(i,j)=2*i+j;  
end;  
end;  
A
### Para o vetor 
     2
     6
    10
    14
    18
    22
    
v(1)=2  
for i=2:6  
v(i)=v(i-1)+4;  
end  
v'  
--- OU ---            
v(1)=2  
for i=1:5  
v(i+1)=v(i)+4;  
end  
v'   
### Para o vetor
           3
           9
          27
          81
         243
         729
        2187
        v(1)=3

for i=2:7  
v(i)=v(i-1)*3;  
end  
v'  
---- or ----  
v(1)=3;  
for i=1:6  
v(i+1)=v(i)*3;  
end  
v'  

### soma de 1 ate 20 de i^3
sum = 0;  
for i=1:20  
sum = sum + i^3;  
end  
sum  

### soma de 1/n^p de 1 até infinito
% 0 < p <= 1 --> diverge  
% p > 1 --> converge  
  
sum = 0;    
for i=1:100000  
sum = sum+1/i^2  
end    
sum    

### Graficos 
  
x=[-10:10];  
y=2*x+3;  
plot(x,y,'r-.d') # red, dash, dot, diamond - also available o, s)  
grid  
xlabel('eixo dos x')  
ylabel('eixo dos y')  
title('grafico de y=2x+3')  
  
x=[-10:10];  
y=x.^2-2*x+3;  
plot(x,y)  
grid  
xlabel('eixo dos x')  
ylabel('eixo dos y')  
title('grafico de y=x²+2x+3')  

### Grafico mais suave, encrementando a cada 0.05  
x=[-10:0.05:10];  
y=cos(x);  
plot(x,y)  
grid  
### Funcoes com restrição - Logaritmos e funções com raiz quadrada
Não possuem negativo, começa em 0:  
x=[0:0.05:10];  
y=log(x);  
plot(x,y)  
grid  

## Exercicios Matlab
### 1
a = 14.75;  
b = -5.92;  
c = 61.4;  
d = 0.6;  
s = a + ((a*b)/c) * ((a+d)^2)/sqrt(abs(a*b));  
s  
### 2 
a = 5*pi/9;  
b = pi/7;  
esquerda = sin(a)*cos(b);  
esquerda  
direita = [sin(a-b)+sin(a+b)]/2;  
direita  

## Aula 3 - Resolução Numérica de Equações não-lineares
### Isolamento das raizes
Se em um ponto A o sinal for oposto de um ponto B, ela passa por 0 um numero ímpar de vezes. Se o sinal for igual, ou não passa nenuma vez ou passa um numero par de vezes.

### Com Gráfico
#### a) f(x) = x³- 9x + 3  
No Matlab:            
x=[-5:0.05:5];  
y=x.^3-9*x+3;  
plot(x,y)  
grid  

#### b) f(x) = √x - 5e^(-x)
No Matlab:  
x=[0:0.05:2];  
y=sqrt(x)-5*exp(-x);  
plot(x,y)  
grid  
