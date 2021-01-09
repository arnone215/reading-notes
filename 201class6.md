# Problem Domain, Objects, and the DOM

## Chapter 3: “Object Literals” (pp.100-105)

*What is an object?*

Objects group together a set of variables and functions to create a model of something you would recognize from the real world. 
#### In an object, variables and functions take on new names!  
- In an object: variables become known as properties. If a variable is part of an object, it is called a **property**. Properties tell us about the object, such as the name of a hotel or number of rooms it has. Each individual hotel might have a different name and a different number of rooms.
- In an object: functions become known as methods. If a function is part of an object, it is called a **method**. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of rooms by booked rooms from the total number of rooms.  
*Programmers use a lot of name/value pairs*:  
- HTML uses attribute names and values.
- CSS uses property names and values.
*In Javascript*:  
- Variables have a name and you can assign them a value of a string, number or Boolean.
- Arrays have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)
- Named functions have a name and a value that is a set of statements to run if the function is called.
- Objects consist of a set of name/value pairs (but the names are referred to as **keys**).

## Chapter 5: “Document Object Model” (pp.183-242)


*The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how Javascript can access and update the contents of a web page while it is in the browser window.*
The DOM is neither part of HTML, nor part of Javascript. It is a separate set of rules. It is implemented by all major browser makers, and covers to primary areas:  

1. Making a model of the HTML page.
When the browser loads a web page, it creates a model of the page in memory.  
The DOM specifies the way in which the browswer should structure this model using a **DOM tree**.  
The DOM is called an object model because the model (the DOM tree) is made of objects.  
Each object represents a diferent part of the page loaded in the browser window.

2. Accessing and changing the HTML page.
The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.  
You will hear people call the DOM an **Application Programming Interface (API)**. User interfaces let humans interact with programs. APIs let programs and scripts talk to each other. The DOM states what your script can ask the browser about the current page, and how to tell the browser to update what is being shown to the user.

