# Basic-Calender
Calendar is a very common element in today's web applications. Whether you are building an event booking application, appointment system or even a social network. Calendar is essential.
Table Of Content
Building the Calendar class
Make it prettier
Final and source code
 Building the Calendar class
Firstly copy the source code below to a class file "calendar.php". We will go through each important function.
This "Calendar" class is a complete object, which will echo a HTML calendar upon calling its "show()" function. Cross month navigation is also handled. This makes it super handy to use.
public function show():This is the only public function Calendar has. This function basically calls each private function below to create the HTML calendar interface.
The basic idea of creating a web calendar is that, firstly it determines how many rows(weeks) to create, and then it loops over the rows and create 7 cells on each row. Meanwhile it puts corresponding day value to the cell according to the day of week (Monday to Sunday).
Take a closer look at each private function below to understand.
private function _showDay():This function will determine what value to put to the created cell. It can be empty or numbers.
private function _createNavi(): This function will create the "Prev" && "Next" navigation buttons on the top of the calendar.
private function _createLabels(): This function will create labels for the day of week. ( Monday to Sunday). You can update the language string to your own choice. But be cautious. You should not change the order of the labels.
private function _weeksInMonth(): This is a tricky function. It can tell you how many weeks are there for a given month. This is used in show() function to create number of rows(weeks).
private function _daysInMonth(); This function tells how many days in a given month.
Functions are working closely to create the PHP calendar. You should follow function show() to understand deeply how exactly they call each. Code is documented. Give yourself some time to read it.
Make it prettier
Now the Calendar class is actually ready.
However it looks messy without some CSS tricks. Let us create a CSS file "calendar.css" to make the calendar look pretty
