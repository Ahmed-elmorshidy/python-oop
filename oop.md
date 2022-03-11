#python summary
in lists 
```python
to add any thing in last of it we use 
>listname.append()


or any position
>listname.insert(position,value)


to check if a value is in lthe list 
>print(value in listname)

```
##oop python
* the constructor always excuted first when we use its class object 
```python
def _name_(self):
    print('welcome')
```
* in constructors we must give the required positional argument .
---
* any value we give to variable in object didn't change the value in the class which we have an object from .
---
*Always if there is a code, we repeat it a lot every time. It is better to make a method and use the duplicate codes so that we give it the number of parameters we want and it returns the required output*
---
### inheritance 
1. it is a class inherite from another one is't attributes and methods .
2. twe can access the attributes of the inherited parent class . 
``` python
>class name1:
      def __INIT__(self,x,y):
        #and block of code here 
>>class name2(name1):
     def meth1(self):
         block of code ...
```
**here we inherited name1 to name2**.
### inheritance >>super
* we use it to inherite construcore from another class  and add  what we want :
```python
>class animal:
     def __init__(self,name):
         self.name= name
class dog(animal):
    def __init__(self,name):
        super(dog,self).__init__(name)
#here we added dog to the constructor in dog class  
```

---
### multiple inheritance
 when we use inherited class to inherite another > will excuted by the first in the inheritance and then the second :
 ```python
 class A:
     def dothis(self):
         print('i am in A')
 class b(A):
     pass
 class c :
     def dothis(self):
         print('i am in c')
 class d(b,C):
     PASS 
 #D>B>A>C                       
 ```
to show steps we use >method.mro()
