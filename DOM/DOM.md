# *0. Adding JS to the html code:*

![[Screenshot 2024-02-10 203446.PNG]]

![[Screenshot 2024-02-10 203352.png]]

 NOTE: Best practice to add the JS script is to add at the very end, because even if there is any problem while loading the JS, the html would have already been loaded.


# *1. Document Object Model:*
Problem statement: To make our site interactive, some parts of the site should change when somebody tries to interacts,

so, the browser will divide the html/document into a DOM tree that will make a family tree 
![[Pasted image 20240213001029.png|200]] ![[Screenshot 2024-02-13 001018.png|200]] 
Here, we can select different objects that will have two properties that is:
1. Property - Things that it describes    ex: for a CAR Object, it properties may be color, shape etc...
2. Methods - Things that it can do        ex: for a CAR Object, it method may be drive, stop etc...
For the above example, 
![[Pasted image 20240213001805.png|500]]
here, using this, we can select the elements as follow:
![[Pasted image 20240213002023.png|150]] For a "BUTTON" object, these are some of its properties and methods


# *2. SELECTING ELEMENTS IN HTML CODE WITH QUERY_SELECTOR*

![[Pasted image 20240213192002.png|200]] Here, there are multiple ways to select the element

## Example: 1
![[Pasted image 20240213192302.png]]
![[Screenshot 2024-02-13 192346.png|100]] ![[Screenshot 2024-02-13 192429.png|100]] Here the H1 has id = "title", and hence, we can select it using 

![[Screenshot 2024-02-13 192425 1.png|400]]getElementByID("ID NAME)

## Example: 2
Selecting Element by tagName, here all element with that tagName will be selected
![[Pasted image 20240213193152.png|500]]

![[Screenshot 2024-02-13 193531.png|100]]![[Screenshot 2024-02-13 193411.png | 100]]Here, Selecting using tagName, we have to specify the element we are targeting, example in this list, to select the 3rd element we use [2] to signify that;

![[Screenshot 2024-02-13 193526.png|500]]

## Example: 3

Note: Here the getElemetnByClassName will select all elements that are in the class, but it select element in array, so we have to specify the element, similar to the above one.

## Example: 4

getElementBySelector() - will make selection in a similar way we were selecting elements in 
CSS styling using
![[Screenshot 2024-02-13 194627.png|280]]    ![[Screenshot 2024-02-13 194633.png|300]]
![[Screenshot 2024-02-13 194644.png|250]]             ![[Screenshot 2024-02-13 194650.png|250]]
we can select any id, class, element, multiple ids, class etc..., similar selection we did in CSS

![[Screenshot 2024-02-13 195602.png|300]]![[Screenshot 2024-02-13 195553.png|400]]
Here, to select this h1, we do as follow and it is selected using querrySelector


#### NOTE: To select specific element
![[Screenshot 2024-02-13 195815.png|500]]![[Screenshot 2024-02-13 195849.png|400]]

Here, "li a", the selector will check for "a" that is inside the "li"

Note: If there are more then one elements that satisfies the selector tag, then it will select only the first one, but to select all in an array, we use querrySelectorAll to select all elements and then can use [position] to select the element specifically;

##### NOTE: DUE TO THE EASE OF USE, WE USE QUERRYSELECTOR and QUERRYSELECTOR


# *3. TO CHANGING STYLE OF SELECTION*

visit w3school - DOM style docs to know about different styles;

![[Screenshot 2024-02-13 201033.png|350]]![[Screenshot 2024-02-13 201108.png|350]]
we can change style by accessing the properties using style word


# *4. SEPERATE STYLE AND BEHAVIOUR*

To separate CSS (style) and JS (Behavior)
### CLASSLIST

we can create different classes of styles in CSS and then can use them onto any element in the HTML using JS
![[Pasted image 20240214234842.png|300]] ![[Pasted image 20240214234852.png|200]]
![[Pasted image 20240214234949.png|400]]
Here, we the .invisible class (CSS) can be applied to the HTML class btn, using JS classList

	SOME TYPES ARE:    classList.add(CLassName);  -- to add the ClassName
					 classList.remove(ClassName);  -- to remove ClassName
					classList.toggle().toggle(ClassName)  --to toggle ClassName

# *5. InnerHTML and InnerTEXT

![[Pasted image 20240215000805.png|400]]

![[Screenshot 2024-02-15 000916.png|350]] Will show the text btw the tag
![[Screenshot 2024-02-15 001019.png|350]] Will show the html code btw tag

and since we can access the html code between the tags, we can change the html code too:

![[Screenshot 2024-02-15 001148.png|550]]

# *6. Manipulating Attributes

Attributes of any element that are inside the tag except the name:
![[Screenshot 2024-02-15 003219.png|500]]
Here, all the attributes can be seen using .attributes, get the attributes value using getAttributes, and setting the attributes using setAttributes
![[Screenshot 2024-02-15 003548.png|500]]



