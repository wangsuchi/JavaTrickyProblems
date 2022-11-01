# JavaTrickyProblems
a list of discussion, answering the confusion of java

1. Is java, a programming language of passing by reference, or passing by value?
https://stackoverflow.com/questions/40480/is-java-pass-by-reference-or-pass-by-value?page=1&tab=scoredesc#tab-top

2. Comparable vs Comparator
→comparable is an interface.If you want to sort a collection of class(using sort() method) based on whatever field of the class, you need to implements comparable interface to that class, and override the compareTo() method to specify your sort logic.

→comparator is also an interface. comparator comes in handy when you can't edit the original sort target class source or you want to implement your own sort logic. 
create an anonymous class of comparator in main class and specify your sort logic, then pass this comparator to
sort() method, which has 2 parameters,one is the sort target list, the other is the Comparator we just created.

fyi,integer,string class has already implemented comparable interface. so we can sort integer directly.

youtube:  https://www.youtube.com/watch?v=oAp4GYprVHM


3. plus/minus-equal operator----- +=/-=
  updates by adding/subtracting the value on the right 
  (easy to mix up: =+ & =-, only act as 正负号)
  
4.  An operation between an integer and another integer will always result in an integer value (it cuts off all decimals).

5. static vs final static modifier
(1)static:  
Whenever we declare variable as static, then at the class level a single variable is created which is shared with the objects. Any change in that static variable reflect to the other objects operations. If we won’t initialize a static variable, then by default JVM will provide a default value for static variable.
(2)final static:
Declaring them as static final will help you to create a CONSTANT. Only one copy of variable exists which can’t be reinitialize.
Initialization of variable Mandatory(compulsory): we have to perform initialization explicitly whether we are using it or not and JVM won’t provide any default value for the final static variable.

https://www.geeksforgeeks.org/final-static-variable-java/

6.
