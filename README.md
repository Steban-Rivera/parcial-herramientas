# parcial-herramientas
## Ejercicio python 
```python
#Información Cliente
print("Digite cédula y rol")
c=int(input())
r=input()
u=""
t=0
q=[]
pp=[]
cc=[]
if r=="estudiante" or r=="Estudiante":
    print("Escriba si o no según corresponda")
    print("Hace parte del programa de becas?: ")
    b=input()
    if b=="si":
        r="becado"
    else:
        r="estudiante"
#Producto a comprar
while u!="no":
    print("Digite código del producto, cantidad a llevar y precio")
    n=int(input())
    q.append(n)
    m=int(input())
    cc.append(m)
    p=int(input())
    pp.append(p*m)
    t+=p*m
    print("Desea comprar algo más?")
    u=input()
if r=="becado":
    tt=t*.5
    t*=.5
elif r=="estudiante":
    tt=t*.3
    t*=.7
else:
    tt=t*.2
    t*=.8
#Salida
if len(q)==1:
    print("El",r,"con cédula",c,"debe pagar",int(t),"por el producto",n)
else:
    print("El",r,"con cédula",c,"esta es su factura:")
    print("Código","cantidad","Total")
    for i in range(len(q)):
        print("  ",q[i],"    ",cc[i],"    ",pp[i])
    print("Total descuento:",int(tt))
    print("Total a pagar",int(t))
           
           
           
```
### Explicacion del programa
#### ¿Que resuelve?
El programa pide cédula y rol de la persona que ingresa
luego pide código, cantidad y precio del producto,
finalmente pregunta si desea llevar otro producto, según
la respuesta se repite el proceso o no.
Finalmente imprime una factura que tiene el código individual
de cada producto con la cantidad y el total neto
en la parte posterior dice el descuento y despuél el total con
eldescuento aplicado.




#### ¿Que modelo computacional lo resuelve
Python.


#### ¿cual es la entrada?
información del comprador e información de los productros.


#### ¿cual es la salida?

Factura con la especificación de los productos.


#### ¿que calcula?

Un total de productos teniendo en cuenta descuentos segúnsu rol.

### Preguntas de control de errores


    

