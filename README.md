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


