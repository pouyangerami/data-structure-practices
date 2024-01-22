def max(lst):
  x=lst[0]
  for i in range (1 , len(lst)):
    if lst[i]> x :
      x= lst[i]
  return x
def f(x,y,n):
  if x>y:
    for i in range (n):
      print(i)
  else:
    for i in range (n):
      for j in range (n):
        print (i , j)

import matplotlib.pyplot as plt

lst = [10,100,1000,10000,100000,1000000]
def avg (s):
  n = len(s)
  A=[0]*n
  for j in range (n):
    total=0
    for i in range(j+1):
      total += s[i]
    A[j]= total/(j+1)
  return A

avg_lst = avg(lst)

plt.plot(avg_lst)
plt.xlabel('index')
plt.ylabel('average')
plt.title('Average value in list')
plt.show()
import matplotlib.pyplot as plt

lst = [1,2,3,4,5,6,7,8,9,10]

def max (lst):
  x = lst [0]
  for i in range(1,len(lst)):
    if lst[i]>x:
      x = lst[i]
  return x

plt.plot(lst)
plt.xlabel('index')
plt.ylabel('value')
plt.title('max value in list')
plt.show()
def disjoint(A,B,C):
  for a in A:
    for b in B:
      if a == b:
       for c in C:
        if a == c:
          return False
def disjoint(A , B , C):
  for a in A:
    for b in B:
      for c in C:
        if (a ==b == c):
          return False
    return True
def r(a):
  n = len (a)
  x = [None]*n
  for j in range (n):
    x[n-1-j]= a[j]
    return x
def r(a):
  n = len (a)
  x = [None]*n
  for j in range (n):
    x[n-1-j]= a[j]
    return x
def r(a):
  n = len (a)
  for i in range (n//2):
    a[i], a[n-1 -i]=a[n-1-i],a[i]
  return a
def respost(Lst) :
  s = stack((len(Lst)) // 2 )
  for e in Lst :
    if e == '*' :
      t2 = s.pop()
      t1 : s.pop()
      t = t1 * t2
      s.push(t)
  else :
    s.push(e)
  return s.stack[0]
def a(n):
  for j in range (n):
   i = 1
   while i <n :

      i *2
def Match_s(str) :
  s=stack()
  for i in str :
    if i in '([{' :
      s.push(i)
    elif i in ')]}' :
      if s.peek() == i :
        s.pop()
      else :
         return False
  if s.is_empty() :
    return True
  else :
    return False
class node :
  def init(self , d):
    self.data = d
    self.nexte = None
class Queue:
  def init (self , k):
    self.k = k
    self.queue=[None]*k
    self.front= -1
    self.rear = -1
class Linkedlist :
  def init(self):
    self.head = None
class Queue:
  def init (self , k):
    self.k = k
    self.queue=[None]*k
    self.front= -1
    self.rear = -1
def display(self) :
  t = node()
  t = self.head
  while (t != None) :
    print (t.data , end = ' --> ')
    t = t.next
    print ('None')
def addinstart (self , data) :
  n = node (data)
  n.next = self.head
  self.head = n
class Queue:
   def disqueue (self):
    if self.front == -1:
      print('empty')
      for i in range (self.front , self.rear+1):
        print(self.queue[i])
def addinend (self , data) :
  n = node(data)
  t = self.head
  if (t == None):
    self.head = n
  else :
    while (t.next) :
      t = t.next
    t.next = n
def insqueue(self , data):
  if (self.rear == -1):
    self.front=0
    self.rear = 0
    self.queue[0]=data
    if(self.rear +1 == self.k):
      print('is full')
      return
    else:
      self.rear +=1
      self.queue[self.rear]= data
class Linkedlist :
  def init(self) :
    self.head = None
  def addafter(self,m,d) :
    n = node(d)
    t = self.head
    while (t.data != m) :
      t = t.next
      t.next = n
def delfirst(self) :
  if(self.head == None) :
    return 'empty'
  else :
    self.head = self.head.next
def dellast (self) :
  if (t== None )
  while (t.next.next != None ) :
    t = t.next
  t.next = None
def delafter (self , m ):
  t = self.head
  while (t.data != m) :
    t = t.next
  t.next = t.nex.next
class dnode :
  def init(self , data) :
    self.data = data
    self.next = None
    self.prev = None
def delqueue(self):
  if (self.front== -1):
    print('empty')
  elif self.front== self.rear:
      t= self.queue[self.front]
      self.front= -1
      self.rear = -1
      return t
  else:
        t= self.queue[self.front]
        self.front= -1
        return t
class dLinkedlist :
  def init (self) :
    self.head = None
  def display (self):
    t =self.head
    while (t !=None) :
      print (t.data ,' <--> ')
      t = t.next
    print('None')
def addinstart (self , d) :
  n = dnode()
  if self.head != None
     n.next = self.head
     self.head.prev = n
  self.head = n
def insqueue_c(self , data ,k):
  if ((self.rear+1)% k ==self.front):
    print ('full')
  elif(self.front== -1):
      self.front=0
      self.rear = 0
      self.queue[self.rear]= data
  else:
      self.rear +=1
      self.queue[self.rear]= data
def addinend (self , d) :
  n = dnode(d)
  if self.head != None :
    t = self.head
    while (t.next != None) :
      t = t.next
    t.next = n
    n.prev = t
  else :
    self.head = n
def delqueue_c(self,k):
  if (self.front== -1):
    print('empty')
  elif self.front== self.rear:
      t= self.queue[self.front]
      self.front= -1
      self.rear = -1
      return t
  else:
        t= self.queue[self.front]
        self.front= (self.front +1)% k
        return t
class stack():
  def init (self,limit =10):
    self.stack =[]
    self.limit =limit
def delfirst(self) :
  if(self.head == None) :
    return -1
  self.head = self.head.next
  self.head.prev.None
def pop(self):
  if len(self.stack)<= 0:
    return -1
  else:
    return self.stack.pop()
def peek(self):
  if len (self.stack)<=0:
    return -1
  else:
    return self.stack[len(self.stack)-1]
def push(self , data):
  if len(self.stack)>= self.limit:
    return -1
  else:
    self.stack.append(data)
def delete (self , data ) :
  if self.head == None :
    print ("empty")
    return
  if self.head.next = self.head :
    if self.head.data == data :
      self.head = None
      return
    return -1
  t = self.head
  while (t .data != data ) :
    p = t
    t = t.next
    if t == self.head :
      return -1
  p.next = t.next
  t.next = None
def display(self):
  if len (self.stack)<=0:
    return -1
  else:
    for i in self.stack:
      print(i)
class BTnode() :
  def init(self , data , left = None , right = None ) :
    self.data = data
    self.left = left
    self.right = right
def dec2bin(number):
  s = stack()
  while number >0:
    r = number%2
    s.push(r)
    number = number//2
    b = ""
  while not s.is_empty():
    b = b +str(s.pop())
  return b
class Btree() :
  def init(self , root = None ) :
    self.rot = root
  def inorder(self , root ) :
    if (root == None ) :
      return
    else :
      self.inorder(root.left)
      print(root.data)
      self.inorder(root.right)
def is_empty(self):
  if len (self.stack)<=0:
    return True
  else:
    return False
def reverse(lst):
  s=stack()
  for e in lst:
    s.push(e)
  for i in range (len (lst)):
    lst[i]= s.pop()
def addafter (self , m , data ) :
  if self.head == None
     return -1
    n = node(data)
    t = self.head
    while t.data != m:
      t = t.next
      if t == self.head :
        return -1
def reverse_stack(s):
  s1=stack()
  s2 = stack()
  while not s.is_empty():
    s1.push(s.pop())
  while not s1.is_empty():
    s2.push(s1.pop())
  while not s2.is_empty():
    s.push(s2.pop())
def delmid(self) :
  t = self.head
  count = 0
  while (t!=None):
    t = t.next
    count += 1
  t = self.head
if count % 2 == 0 :
  for i in range ( count // 2) :
    t = t.next
else :
  for i in range (count //2 +1) :
    t = t.next
  t.next.prev = t.prev
  t.prev.next = t.next
  t.next = None
  t.prev = None
class cLinkedlist :
  def init(self) :
    self.head = None
  def display(self) :
    t = self.head
    if t is None :
      print("empty")
      return
    while t.next != self.head :
      print(t.data , end = ' --> ')
      t = t.next
    print(t.data)


