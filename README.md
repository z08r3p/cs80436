java c
Faculty of Arts  Science 
Fall 2024 Quiz 10 - V1 
CSC 110 Y1F
Question 1. Classes            [6   marks] Part (a) [2   marks]
Complete   the   init   in   the   following   Pet   class   according   to   the   provided   description:
class Pet:
"""A virtual pet that   can be fed   and   cuddled   .
A pet has a certain hunger   level, measured   as   an   integer,
where higher values indicate   a hungrier pet   .
Additionally, the pet has a happiness level, which increases when   the   pet   is   cuddled   .
Instance Attributes:
- name:   the   pet   '   s   name
- hunger: the   pet   '   s   hunger   level   (starts   at   5)   .
- happiness: the   pet   '   s   happiness   level   (starts   at   0)   .
Representation Invariants:
- 0   <= self .hunger <= 10
- 0   <= self .happiness
"""
name:   str
hunger:   int
happiness:   int
def   init   (self, name:   str) ->   None:
"""Initialize a new pet with the given name, hunger level   5   and   happiness   level   0   .
>>> p   =   Pet(   '   Bumbly   '   )
>>> p   .name
'   Bumbly   '
>>> p.hunger
5
>>> p.happiness
0
"""
# TODO: complete   this method body
We   want   to   add   a   few   more   methods   to   the   Pet   class   from   the   previous   page.      Complete   the   methods   below   according   to   the   provided   descriptions:
Part (b) [4   marks]
def   feed(self)   -> None:
"""Feed   this   pet, decreasing   its   hunger   level   by   1   (to   a   minimum   of   0)   .
>>> p   =   Pet(   '   Strawberry   '   )
>>> p.feed()
>>> p.hunger
4
"""
# TODO: complete   this method body
def cuddle(self, minutes:   int) ->   None:
"""
Cuddle this pet, increasing its happiness level   by   1   for   every   5   minutes   of   cuddle   time   .
(If minutes is not divisible by   5,   ignore   any remainders.)
>>>   p   =   Pet(   '   Mia   '   )
>>> p.happi代 写CSC 110 Y1F Fall 2024 Quiz 10 - V1Python
代做程序编程语言ness
0
>>> p.cuddle(33)   >>> p.happiness      6
"""
# TODO: complete   this method body
Question 2. Stacks         [4   marks]Complete   the   following   function   that   takes   in   a   Stack   object.   You   may only use the public Stack methods as   provided   on   the   reference   sheet:      is_empty,   push,   and   pop.   Do   not   call   any   method   besides   these   three.   You   may   also   create   a   new   Stack   if necessary.
def peek(stack: Stack) ->   Optional[Any]:
"""Return the top   item on   the   given   stack   .
If the stack   is   empty,   return   None   .
This function should leave the   stack unchanged when   the   function   ends   .
>>>   stack   =   Stack()   >>>   stack.push(1)
>>>   stack.push(2)   >>> peek(stack)
2
>>>   stack.pop()   2
"""
# TODO: Implement   this   function   .
Question 3. Queues         [4   marks]
Below   is   a   function   that   is   missing   most   of its   docstring.   You   will   provide   additional   pieces.    Assume   the   Queue   class   is   a   concrete   implementation   of the   Queue   ADT   we   discussed   in   class.
def   mystery(q1: Queue, q2:   Queue)   -> Queue:
"""
Preconditions:
- q1   and   q2   contain   only   ints """
q =   Queue()while   not   q1   .is_empty():   item1 =   q1.dequeue()   item2 =   q2.dequeue()
if   item1   >   item2:
q.enqueue(item1)   else:
q.enqueue(item2)
return   q
Part (a) [2   marks]
What   additional   preconditions   are   needed   to   ensure   the   function   does   not   raise   an   error?   If none   are   necessary,   write   “None". (Note:    You may write the precondition in plain English; Python code is not necessary.) 
Part (b) [2   marks]Write   a   plain   English   description   of the   function,   suitable   for   the   docstring.   Assume   all   preconditions   are   met.




         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
