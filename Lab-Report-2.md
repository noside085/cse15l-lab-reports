# Lab Report 2

## Part 1

Code for StringServer:

![Image](L21.png)

First `/add-message?s=<String>` to the server:

![Image](L23.png)

In this `/add-message?s=<String>`, the method "handleRequest" is called. The argument relevant to our method is 
"localhost:805/add-message?s=Hi,%20this%20is%20Edison", which is my URL. The fields that are relevant in the 
method would be `ArrayList<String> list` and `String allStrings`. `list` is used to store all the given strings
by the user, and `allStrings` is a string that contains all the strings currently stored in `list`, which is used 
to be presented to the user to show all the currernt strings on the website. From this specific request, `list` is updated 
from having no strings stored to then store the string "Hi, this is Edison.". Then `allStrings` is updated to become
"Hi, this is Edison.".

Second `/add-message?s=<String>` to the server: 

![Image](L22.png)

In this `/add-message?s=<String>`, the method "handleRequest" is called. The argument relevant to our method is 
"localhost:805/add-message?s=This%20is%20my%20String%20Server", which is my URL. The fields that are relevant in the 
method would be `ArrayList<String> list` and `String allStrings`. `list` is used to store all the given strings
by the user, and `allStrings` is a string that contains all the strings currently stored in `list`, which is used 
to be presented to the user to show all the currernt strings on the website. From this specific request, `list` is updated 
from having one string ("Hi, this is Edison.") to having two string, where the second string is "This is my String Server".
Then `allStrings` is updated to become "Hi, this is Edison. /n This is my String Server".

## Part 2

Code with Bug:

l25

Failure Inducing Input:

	public void testReverseInPlace() {
		int[] input1 = { 3 };
    		ArrayExamples.reverseInPlace(input1);
    		assertArrayEquals(new int[]{ 3 }, input1);

    		int[] input2 = { 1, 2, 3, 4, 5 };
    		ArrayExamples.reverseInPlace(input2);
    		assertArrayEquals(new int[]{ 5, 4, 3, 2, 1 }, input2);
	}
	
