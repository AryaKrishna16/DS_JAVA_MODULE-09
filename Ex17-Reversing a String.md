# Ex17 Reversing a String Using Stack Data Structure
## AIM:
To write a Java program that reverses an input string using a stack, without using built-in reverse functions.

## Algorithm
Start the program.
Read the input string from the user.
Create an empty stack of characters.
Traverse the string and push each character onto the stack.
Pop each character from the stack and append it to a new string — this gives the reversed string.
Display the reversed string.
Stop the program.
## Program:
```
/*
Program to reverses an input string using a stack
Developed by: E ARYA KRISHNA 
RegisterNumber:  212225240014
*/
import java.util.Scanner;
import java.util.Stack;

public class ReverseStringWithStack {

    public static String reverseString(String input) {
         Stack<Character> stack=new Stack<>();
        for(char ch:input.toCharArray())
        {
            stack.push(ch);
        }
        StringBuilder rev=new StringBuilder();
        while(!stack.isEmpty())
        {
            rev.append(stack.pop());
        }
        return rev.toString();
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();
        String reversed = reverseString(input);
        System.out.println(reversed);

        scanner.close();
    }
}
```

## Output:
<img width="452" height="162" alt="image" src="https://github.com/user-attachments/assets/8c99fc61-46a6-4a34-b3fe-4fbfc49095f1" />



## Result:
Thus, the program successfully reverses the given string using a stack without relying on built-in reverse functions.
