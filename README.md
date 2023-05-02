Download Link: https://assignmentchef.com/product/solved-comp3522-assignment-2-the-supply-chain
<br>
<span style="font-size: 2.61792em; letter-spacing: -1px;">Introduction</span>

The second COMP 3522 assignment for the semester is here!

In this assignment you will be moving beyond the Python Fundamentals and start writing systems that include Design Patterns! You will be working in groups of two (2) for this assignment. So find a partner, and create a <strong>NEW</strong> Github repo for this assignment. (I don’t want anyone else having access to your personal COMP3522 repo except yourself). Name this GithubRepo COMP3522_Assignment2_A########_A######## , where A######## is the student ID number of the group members.

For this assignment we will be simulating a store that keeps festive seasonal items all year long.

That is, it keeps a stock of toys, stuffed animals, and candy that vary by holidays (Easter, Christmas and Halloween). So if you ever wanted easter eggs in december, this would be the place to go!

Your code will be taking in bulk orders that come in from the store’s website in the form of excel files. The system should implement the abstract factory pattern to achieve this.

When going through the assignment brief start drawing out a preliminary UML class diagram to identify all the classes, attributes and any behaviors that you may need. A draft diagram should be made before you start writing any code. Be creative and enjoy the process! I encourage you to come discuss your designs with me if you want any feedback.

<h1>Submission Requirements</h1>

<ol>

 <li>This assignment is due before <strong>11:59 PM on Sunday 22nd March 2020. If you want me to check any commits past this date, the total grade will incur a penalty.</strong> The penalty for late submissions will be 5% of the total grade per day that it is late.</li>

 <li>Submit your .py files and UML diagrams in a separate GitHub repository following the naming convention <em>COMP3522_Assignment2_A########_A########</em> , where <em>A########</em> is the student ID number of the group members..</li>

 <li>This is an group assignment. All code must be written by the group members only. I encourage you to discuss and share ideas with your friends but remember to write your own code!</li>

 <li>Include a Readme file that describes how your application works and if there are any errors or use cases that have limitations or if it doesn’t meet any of the requirements. This is also the spot where you want to document any features (the ones specified in this assignment and any extra features) that you may or may not have implemented. This will help me keep an eye out for them as I grade your work.</li>

</ol>

<h1>Grading</h1>

The assignment is marked out of <strong>24</strong>. For full marks, you must:

<ol>

 <li>Correctly implement the requirements described in this document – <strong>10 Marks</strong></li>

 <li>Correctly format and comment your code. Eliminate all warnings offered by PyCharm, follow PEP 8 and PEP 257 guidelines, use good function and variable names, write code that is easy to understand, use whitespace wisely, write good and appropriate docstrings, etc. – <strong>2 Marks</strong></li>

 <li>Structure/design your classes to maximize code re-use, make it readable and maintainable. Follow the SOLID principles and the Law of Demeter. <strong>– 4 Marks</strong></li>

 <li>Submit a UML Class Diagram depicting appropriate use of OOP principles, inheritance and design in your code- <strong>2 Marks</strong></li>

 <li>Submit a UML Sequence Diagram depicting the flow of control when an order is ringed in. <strong>– 2 Marks</strong></li>

 <li>Handle errors and unexpected player behavior (read: input) gracefully using the Easier to Ask for Forgiveness philosophy. – <strong>3 Mark</strong></li>

 <li>Format your output. Make sure your messages display the correct information in a pleasant, readable manner. You could even use ASCII art if you dare! – <strong>1 Mark</strong></li>

</ol>

Please remember that this is a group assignment. Any code/ascii art taken from the web must be referenced/cited!

Good luck, and have fun!

<h1>Implementation Requirements</h1>

Your storefront (give your store a name!) should implement the following features.

<h2>The User Menu</h2>

When the program runs, it should provide a terminal menu that the store owner would have access to. The menu should let the cashier.

<ul>

 <li><strong>Process Web Orders</strong></li>

</ul>

At the end of each day the store owner downloads an excel file of all the online orders placed that day and process them through the system.

<ul>

 <li><strong>Check Inventory</strong></li>

</ul>

This allows the cashier to check what is currently in stock and will also provide a status indicator for each items that indicate if the stock for this item is <strong>LOW</strong>, <strong>VERY LOW</strong>, <strong>IN STOCK, or</strong> OUT OF STOCK.

o    In Stock – 10 or more items in stock o       Low – Less than 10 items o     Very Low – Less than 3 items o       Out of Stock – 0 items

<ul>

 <li><strong>Exit</strong></li>

</ul>

Exits the program and prints out the daily transaction report.

<h2>The Inventory</h2>

The store maintains the following items:

<h3>Toys</h3>

For each festive season, the store stocks a unique toy. Despite that, there are some properties of each toy that all toys have in common. These are:

<ul>

 <li>Whether the toy is battery operated or not.</li>

 <li>The minimum recommended age of the child that the toy is safe for.</li>

 <li>A name</li>

 <li>A description</li>

 <li>Product ID (A unique combination of letters and numbers)</li>

</ul>

The holiday specific toys are:

<ol>

 <li><strong>Santa’s Workshop</strong></li>

</ol>

The premium Christmas present, this is not a battery operated toy. The doll house comes in different varieties. They can vary in:

<ul>

 <li>dimensions (width and height) o The number of rooms</li>

</ul>

<ol start="2">

 <li><strong>RC (Remote Controlled) Spider</strong></li>

</ol>

The RC Spider is the toy to get during Halloween. This toy is is battery operated. The different varieties of spiders that are sold have the following properties:

<ul>

 <li>Speed o Jump height o Some spiders glow in the dark, while others do not. o       The type of spider – This can either be a Tarantula or a Wolf Spider and nothing else.</li>

</ul>

<ol start="3">

 <li><strong>Robot Bunny</strong></li>

</ol>

The Robot Bunny is the toy for toddlers and infants out there. The toy is battery operated. These come in different varieties as well! Their properties are:

<ul>

 <li>The number of sound effects o The colour – This can be either Orange, Blue, or Pink and nothing else. <strong>Stuffed Animals </strong></li>

</ul>

All stuffed animals have the following attributes:

<ul>

 <li>Stuffing – This can either be Polyester Fiberfill or Wool</li>

 <li>Size – This can either be Small, Medium or Large</li>

 <li>Fabric – This can either be Linen, Cotton or Acrylic</li>

 <li>Name</li>

 <li>Description</li>

 <li>Product ID</li>

</ul>

The holiday specific stuffed animals are: 1. <strong>Dancing Skeleton</strong>

The dancing skeleton is made out of Acrylic yarn and stuffed with Polyester Fiberfill. This skeleton is sure to add to your Halloween decorations.

o    The dancing skeleton also <strong>glows in the dark</strong>.

<ol start="2">

 <li><strong>Reindeer</strong></li>

</ol>

The reindeer comes with its very own personal mini sleigh and is the stuffed animal for Christmas. It is made out of Cotton and and stuffed with Wool.

<ul>

 <li>Has a glow in the dark nose.</li>

</ul>

<ol start="3">

 <li><strong>Easter Bunny</strong></li>

</ol>

The Easter Bunny is made out of Linen and stuffed with Polyester Fiberfill.

<ul>

 <li>It comes in different <strong>colours</strong> – White, Grey, Pink and Blue and nothing else.</li>

</ul>

<h3>Candy</h3>

All candies have the following properties:

<ul>

 <li>A flag to check if it contains any nuts</li>

 <li>A flag to check if it is lactose free.</li>

 <li>Name</li>

 <li>Description</li>

 <li>Product ID</li>

</ul>

The holiday specific candies are:

<ol>

 <li><strong>Pumpkin Caramel Toffee</strong></li>

</ol>

The Pumpkin Caramel Toffee is Halloween themed and is not lactose free and may contain traces of nuts.

<ul>

 <li>It comes in two varieties — <strong>Sea Salt</strong> and <strong>Regular</strong>.</li>

</ul>

<ol start="2">

 <li><strong>Candy Canes</strong></li>

</ol>

Candy Canes are Christmas themed. It is lactose free and does not contain nuts.

<ul>

 <li>The stripes on the candy cane can either be <strong>Red</strong> or <strong>Green</strong></li>

</ul>

<ol start="3">

 <li><strong>Creme Eggs</strong></li>

</ol>

Creme Eggs are Easter themed and are not lactose free and may contain traces of nuts.

<ul>

 <li>Pack Size – The creme eggs come in different packets, each containing a different number of creme eggs.</li>

</ul>

<h2>Process Web Orders</h2>

The store owner can go to their online storefront and download the orders received during the day in the form of an excel sheet.

Your code must prompt the user for the name of this file and use the pandas package to read in them in and process the order. The store owner can do this multiple times a day if need be. I recommend you create variations of the excel file that I have provided and use it to test your program.

Your code must contain an OrderProcessor class that is responsible for reading each row of these files and creating and yielding an Order object. The OrderProcessor class contains a FactoryMapping which maps the holiday to the appropriate factory class.

Each Order contains the following:

<ul>

 <li>Order number</li>

 <li>Product ID</li>

 <li>Item – The type of item (Toy, StuffedAnimal and Candy).</li>

 <li>Name of the item</li>

 <li>A dictionary of product details. These details are the rest of the attributes of the item as specified in the excel sheet <strong>EXCEPT</strong> the name of the holiday — Easter, Christmas or Halloween.</li>

 <li>The order should also contain a reference to the appropriate Factory object that can create this item.</li>

</ul>

Now, on to the important bits, what happens with these Order objects?

They are sent to the store (more on the store below). The store should find the item in its inventory and reduce the quantity accordingly. In the event an item is not found, the store can use the corresponding factory sent as part of the order to order more items. (More on this below).

<h2>The Storefront</h2>

Your system should contain a Store class that should be responsible for:

<ul>

 <li>Receiving orders and maintaining its inventory</li>

 <li>Getting items from a factory class if the store does not have enough stock</li>

 <li>Creating the Daily Transaction Report</li>

</ul>

The first time the store receives an order for an item, it is likely that it won’t have the item in it’s inventory since the store should be initialized with an empty inventory.

In the event the store receives an order for an item that it does not have inventory for, then it should go ahead and get a 100 of those items made by the corresponding factory class.

<h2>Daily Transaction Report</h2>

When the user chooses to exit the program, the program should write the Daily Transaction Report to a text file. The file specifies the list of orders processed that day.

The text file should follow the naming convention DTR_DDMMYY_HHMM.txt where DDMMYYY refers to the date, month and year (for example, 19th Feb 2020 would be 1902020) and0 HHMM refers to the hour and minute (for example 1:30pm would be 1330).

Be sure to follow the formatting in the example below:

HOLIDAY STORE – DAILY TRANSACTION REPORT (DRT)

05-03-2020 17:58




Order 102, Item StuffedAnimal, Product ID H9405S, Name “Skelly the Tap Dancer”, Quantity 3

Order 103, Item Toy, Product ID T2134C, Name “Santas Workshop Deluxe

Edition”, Quanity 20

Order 104, Item Toy, Product ID T3243H, Name “Terrifying Tarantula”, Quantity

17

Order 105, Could not process order data was corrupted, InvalidDataError –

Stuffing can only by “Polyester Fiberfill” or “Wool”

<h2>Concluding Thoughts</h2>

Remember to approach your code in an object-oriented fashion. Don’t just start bashing out code and hoping that it will all work out. Take a planned approach and consider these steps.

<ol>

 <li>Identify your Product Families and Variations. This is key to getting the Abstract Factory Pattern down.</li>

 <li>Draw our the Product Hierarchies and the Factory Hierarchies.</li>

 <li>Identify any other classes and objects you will need. Figure out what each class is responsible for.</li>

 <li>Draw a UML class diagram showing how the classes/objects relate to each other. Write down the attributes and methods. o       At this stage you can do a simple sketch on paper. Don’t worry about syntax and only mention the important attributes/methods.</li>

 <li>Write some code</li>

 <li>Repeat from step 3. (Take an iterative approach!)</li>

</ol>

When creating your <strong>final</strong> UML diagram, be sure to check syntax, and mention all the attributes and methods.


