Get Blog from the Repository
============================

Lets take a look into the BlogRepository and travel into the inner core of our 
action island.

[CODE Here]

The code is not shortened. The BlogRepository simply does not have any own code 
since all methods which are used very often are already implemented in the 
parent class TX_Extbase_persistence_Repository. These functions are also 
available in all child classes. We call the method findAll(), to retrieve all 
Blog-objects

Excursion: The Repository
-------------------------

The way a repository works is much like a library of a university which works in 
the following way:

You tell an employee of the library to find a book matching certain criteria. 
After a few minutes (or days) you get the corresponding book.

In this case it doesn't matter to you if the book is right below the counter, in 
a shelf, in the cellar, or is not even printed yet (except from the time issue - 
but students have time). It is only important that you get the book.
Remarks made with a pencil by you will be added permanently (hopefully without 
changes) when you return the book.

Translated to a repository:

Via a repository you tell a method to find an object matching certain criteria. 
After a few milliseconds (or seconds) you receive the corresponding object.
In this case you don't care where the object is stored. Practically it even 
doesn't matter if the object is stored in the memory, must be fetched from the 
hard drive, is retrieved via web service from another server, or is instantiated 
for the first time (except from the speed - but users have time). The only 
important thing is that the object is instantiated and delivered to you.
Object attributes changed by you will be stored when you leave the extension.

Kasten:

Although you don't need to implement your own logic extbase expects an existing 
class.