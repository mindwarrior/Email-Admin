note: We create all the required data types like string firstName, string 
lastName etc. but we ENCAPSULATE them by adding private so somebody 
could not change them directly and instead have to use the email API 
which we are built.

### Abstract class in Java
Def: A class which you can't create objects from. It is only useful for
polymorphism and inheritance. Concrete classes are the ones which you 
can create objects from. To use abstract classes you have to extend them.

### Abstract method in Java
Abstract method is a method which must be overridden. It can be an empty method body of which is declared in the method which overrides it.

### Inheritance
When one object acquires all the properties and behaviour of a parent
object. It provides code reusability. It is used for runtime polymorphism(using extends and interfaces).

### Polymorphism
When one task is performed by different ways.
(Use method Overloading and method Overriding).


#### Ex 84:
Write a Java program to take the last three characters from a given 
string and add the three characters at both the front and back of the string. 
String length must be greater than three and more. Go to the editor
Test data: "Python" will be "honPythonhon"

package excercises;

public class Ex84 {
	public static void main(String[] args) {
		
		String str = "Python";
		int sublength = 3;
		if (sublength > str.length() ) {
			sublength = str.length();
		}
		
		String subpart = str.substring(str.length()-3);
		System.out.println(subpart + str + subpart);
		

	}

}

#### Ex 92 
Write a Java program to count the number of even and odd elements in a given array
 of integers

 public class Ex92 {
	public static void main(String[] args) {
		
		int[] nums = {1,5,8,3,2,0,8,1,3};
		int countevn = 0;
		int countodd = 0;
		System.out.println("Original Array:" + Arrays.toString(nums));
		for (int i=0;i<nums.length;i++) {
			if(nums[i]%2 ==0) {
				countevn++;
			}
			else
				countodd++;
		}
		
		
		System.out.println("\nNumber of even elements in Array:" + countevn);

  ### this keyword is a reference variable that refers to the current object.

ArrayList is a non-primitive datatype. Basically, it is an object with ordered collection.
You cannot create an ArrayList of primitive types like int, char etc. You need to use boxed types like Integer, Character, Boolean etc.
Other non-primitive data types are String, Array and object. Basically, any datatype which has methods is a non primitive datatype.
java.util.Collections has following datatypes:
Set:HashSet, LinkedHashSet, TreeSet(sorted set)
List:ArrayList, Vector, LinkedList(it is both a list and queue)
Queue:PriorityQueue.


>Singleton design pattern in java:
It ensures there is only one instance of a class using  a private constructor. Class can be either initialized when the class is created or until the time it is needed.

