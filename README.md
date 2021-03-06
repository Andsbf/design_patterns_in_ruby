This repository includes my notes/code from *Design Patterns in Ruby, by Russell A. Olsen*

GoF patterns covered:
_____________________

- Every pattern has a problem that it is trying to solve. For example, perhaps your code always wants to do exactly the same thing, except at step 44. Sometimes step 44 wants to do this, and sometimes it wants to do that. Perhaps you need a **Template** Method.

- Maybe it is not step 44 that wants to vary but the whole algorithm. You have a well-defined job, something that needs to get done, but there are a lot of ways to do it. You might need to remove the outer covering from a feline creature, and there is more than one technique you might employ. You might want to wrap those techniques—those algorithms—in a **Strategy** object.

- What if you have a class A, which needs to know what is happening over there in class B? But you don’t want to couple the two classes together because you never know when class C (or even class D!) might come along. You might want to consider using the **Observer** pattern.

- Sometimes you need to treat a collection of objects just like a single object—I can delete or copy or move an individual file, but I can also delete or copy or move a whole directory of files. If you need to build a collection of objects that looks just like one of the individual objects, you probably need the **Composite** pattern.

- Now suppose you are writing some code that hides a collection of objects, but you don’t want the collection hidden too well: You would like your client to be able to access the objects in your collection in sequence without knowing how or where you have stored those objects. You definitely need the **Iterator** pattern.

- Sometimes we need to wrap instructions in a kind of a postcard: Dear database, when you get this, delete row number 7843. Postcards are hard to come by in code, but the **Command** pattern is tailor made for this situation.

- What do you do when an object does what you need it to do, but its interface is wrong? Your interface mismatch might be very deep and complex, or it might be as simple as needing an object that can write but having an object that calls it save. The GoF would recommend an **Adapter** to you.

- Maybe you have the right object, but it is over there, someplace else on the network, and you don’t want the client code to care about its location. Or perhaps you want to delay creating your object as long as possible, or control access to it. In this circumstance, you may need a **Proxy**.

- Sometimes you need to add responsibilities to your objects on the fly, at runtime. If you have a need for objects that implement some core capabilities but must sometimes take on additional responsibilities, perhaps you need the **Decorator** pattern.

- Perhaps you have an instance of a class, and it needs to be the only instance of that class—that is, the single instance that everybody uses. Sounds like you have a **Singleton**.

- Now suppose you are writing a base class, one that is meant to be extended. As you are happily coding away at your base class, you realize that it needs to produce a new object and only the subclass will know exactly which kind of object to produce. You may need a **Factory** Method here.

- How do you create families of compatible objects? Suppose you have a system that models various types of cars, but not all engines are compatible with all fuel or cooling systems. How do you ensure that you don’t end up with the automotive equivalent of Frankenstein’s monster? You might build a class devoted to creating all of those objects and call it an **Abstract** Factory.

- Perhaps you are building an object so complex that its construction requires a significant bit of code. Even worse, the process of construction needs to vary according to the circumstances. Perhaps you need the **Builder** pattern?

- Ever have the feeling that you are using the wrong programming language to solve your problem? As crazy as it sounds, perhaps you should stop trying to solve your problem directly and build an **Interpreter** for a language that solves your problem more easily.
