# Java-II-Task-2
grade recevied 97%
Assignment 2 – The FacebookUser Class
We’re going to make a small change to the UserAccount class from the last assignment by adding a new method:
public abstract void getPasswordHelp();
This method is abstract because different types of user accounts may provide different types of help, such as providing a password hint that was entered by the user when the account was created or initiating a process to reset the password.
Next we will create a subclass of UserAccount called FacebookUser. The FacebookUser class needs to have the following fields and methods in addition to what is in UserAccount:
String passwordHint
ArrayList<FacebookUser> friends
void setPasswordHint(String hint)
void friend(FacebookUser newFriend)
void defriend(FacebookUser formerFriend)
ArrayList<FacebookUser> getFriends()
The friend method should add the FacebookUser argument to the friends ArrayList (if that FacebookUser is already in the friends list, display an error message), and the defriend method should remove the FacebookUser argument from that ArrayList (if that FacebookUser is not in the friends list, display an error message). The getFriends method should return a copy of this user’s friends – create a new ArrayList with the same FacebookUsers in it as this user’s friends. Do not return the friends ArrayList directly, since this violates the principle of encapsulation. The getPasswordHelp method should display the passwordHint.
The FacebookUser class should also implement the Comparable interface. FacebookUsers should be sorted alphabetically by username, ignoring capitalization. (Hint: notice that the toString method returns the username of the UserAccount.)
Finally, write a driver program that creates several FacebookUsers and demonstrates the user of the setPasswordHint, friend, defriend, getFriends, and getPasswordHelp methods. Also, put the FacebookUser objects into an ArrayList, sort them (see the jar file for this topic for help on this), and print them out in sorted order.
You will be graded according to the following rubric (each item is worth one point):
• The UserAccount class is abstract and has the requested fields and methods. Only the getPasswordHelp method is abstract.
• The FacebookUser class extends UserAccount
• FacebookUser has a friends ArrayList and methods to add, remove, and
display the friends
• FacebookUser implements Comparable and sorts alphabetically on
username, ignoring capitalization
• FacebookUser has a passwordHint that can be set through a method and is
displayed by the getPasswordHelp method
• The driver program creates a list of FacebookUsers
• The driver program sorts and displays the lists of FacebookUsers
• The driver program exercises the setPasswordHint, friend, defriend,
getFriends, and getPasswordHelp methods
• The program compiles and runs
• The program is clearly written and follows standard coding conventions
