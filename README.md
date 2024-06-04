/1/ Purpose of App

  1. To store, view, and edit a database of Events in a way that is easy for a user to access and modify.

/2/ Current state of App

  1. connected to persistent database
  2. can create Events, Categories, and Tags that can be add and related to each other
  3. can not edit or delete Tags or Categories
  4. can view all Events, Categories, or Tags


/3/ Future impprovements for App

1.Add a Person class 
  1. that exstends to AbstractEntity
  2. has a many-to-many relation to Event class
  3. contains fields for name, age, location, diet preferences, event types, and tags
  4. add needed constructor, getters and setters, as well as any annotations need for fields
<img width="503" alt="image" src="https://github.com/chrimcha/CodingEventsJava/assets/147195321/eb242336-492d-47c6-a836-fe7f48bc20f0">

  5. implement edit and delete for Tags and Categories
  6. Person class will allow user to save Events, Categories, and Tags to their profile for further use

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

/From Text/ Check your solution
Here is an example of how the README may turn out:

1. Our Person class might hold the following fields:
   
    1. id (int) - the unique user ID
    2. firstName (String) - the user’s first name
    3. lastName (String) - the user’s last name
    4 .email (String) - the user’s email, which will also function as their username
    5. password (String) - the user’s password
       
  The class would need getters for all of these fields.
  It could have setters for all fields except id (since it shouldn’t change).

3. The Person class might also have the following references:
   
    1. PersonProfile - a class to gather up all of the profile information about the user
    2. List<Events> eventsAttending - to store events the user wants to attend
    3. List<Events> eventsOwned - a different list, to store the events the user has created
       
  Person would have a many-to-many relationship with Event via List<Events> eventsAttending.
  It would have a one-to-many relationship with Event via List<Events> eventsOwned.
