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
