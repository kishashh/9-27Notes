# 9-27&29Notes

+ public
- private
# protected
~ Package
static = underlined
abstract = italic
constant = ALL-CAPS

Public intercave of a class is a promise to users of class
Superclass makes certian promisesabout avaible methods and instance variables
promises must be kept by all child classes

public abstract class Produce{
...
}

Produce P =new Produce(); will not wbe instantiated
Produce p = new Apple(); knows to inhearet with abstract

A class that extends an abstract class must implement all abstract methods or also be abstract

Propertiesof Abstract classes:
- Must provied constructors
  - protected of private
  - child classes can refrence these with super()
  - could be the default constructor
 - In the abstract superclass
  - provide as many method implementations as possible
  - These implementations may call abstract methods
 
"Multiple" Inheritance
Clone is not just a copy of the object memory, but of all of its component objects
Cloneable requires the implimentation of a clone() method that produces the copy
 
An interface defines no implementation - only a set of abstract methods

A class can implement any number of interfaces
T is a placeholder for any class name


import java.util.Collections;

public class Person implements Comparable<Person> {
    private String firstName;
    private String lastName;
    private String phoneNumber;
    
    public int compareTo(Person o) {
      if(this.lastName.compareTo(o.getLastName()) == 0){
        return this.firstName.compareTo(o.getLastName());
      }
      return 0;
    }
    private String getFirstName(){
      
    }
}
