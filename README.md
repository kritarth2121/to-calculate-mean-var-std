import numpy
a,b=input().split()
a=int(a)
b=int(a)
ar=[]
for i in range(a):
    c=list(map(int, input().split()))
    ar.append(c)
ar=numpy.array(ar)
numpy.set_printoptions(legacy='1.13')
print(numpy.mean(ar, axis = 1))        
print(numpy.var(ar, axis = 0))        
print(numpy.std(ar, axis = None))
