# sololearn Q/A

- [java](#jav)



## Java
### variables

Q. You are given code which outputs the properties of a vehicle, but something is wrong.

Task
Fix the code to print the properties.

Output
Name: Toyota
Engine: 4.7
Year: 2019

```
public class Program
{
    public static void main(String[] args) {
        //fix the variable types 
        String  name = "Toyota";
        String engine = "4.7";
        String year = "2019";
       
        System.out.println("Name: " + name);
        System.out.println("Engine: " + engine);
        System.out.println("Year: " + year);

	}
}
```

### java comments

Q. You are given lines of commented code. Uncomment the required lines in order to have a "Java is awesome" output.

``` 

public class Main {

   public static void main(String[] args) {
       //uncomment necessary line(s)
      // System.out.println("Java is lame");
       System.out.println("Java is awesome");
       //System.out.println("Please uncomment me!!! ^^");
   }
}

```

### primitive operators
Q. A bartender sold 64 bottles of beer and 23 bottles of whisky. You need to calculate how many total bottles are sold.

Task
Calculate and output the total number of sold bottles.

```

public class Program
{
    public static void main(String[] args) {
	int beer  = 64;
        int whisky = 23;
       //calculate the sum and outputit
       System.out.print(beer+whisky);
        
	}
}

```

### increment & decrement 

Q. Tom and Bob are playing a board game, in which both players start with the same number of points. Tom won the first game and got 1 point, while Bob lost the game, and therefore lost 1 point.

You are given a program that is intended to take the initial score and increase Tom's score by 1 and decrease Bob's score by 1.
But something is wrong: the program outputs the scores without the change.

Task
Fix the program to result in the expected outputs.

Sample Input
5

Sample Output
Round 1 results: 
6
4

Explanation
Both players had 5 points at the start of the game. After the first game, Tom gained 1 point (6, the first outputted number), and Bob lost 1 point (4, the second outputted number).


```
import java.util.Scanner;

public class Main {

   public static void main(String[] args) {
       
       Scanner scanner = new Scanner(System.in);
       //taking initial score
       int initScore = scanner.nextInt();
       int scoreTom = initScore;
       int scoreBob = initScore;
       
       System.out.println("Round 1 results:");
       //fix
       System.out.println(++scoreTom);
       System.out.println(--scoreBob);
   }
}

```

## Time converter

Q. You need a program to convert days to seconds. 
The given code takes the amount of days as input. Complete the code to convert it to seconds and output the result.

Sample Input:
12

Sample Output: 
1036800

```

import java.util.Scanner;

public class Program {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		int days = scanner.nextInt();
		System.out.println(days*24*60*60);
		//your code goes here
		
	}
}

```










### Nested if Statements

Q. The sales manager decided to give a gift card to the customers whose purchases total more than 15000. On top of this, the customers whose total purchase is above 30000 will receive a second gift card.
You are given a program, which takes the purchase amount as input, and print "Gift card" if it is above 15000.

Task
Complete the code to print "Gift card" again if the purchase is above 30000.
 
Sample Input
36000

Sample Output
Gift card
Gift card


```
import java.util.Scanner;

public class Main {
   public static void main(String[] args) {
       Scanner read = new Scanner(System.in);
       int purchases = read.nextInt();
       
       if(purchases > 15000){
        System.out.println("Gift card");
        //complete the code
        
        }
        if(purchases > 30000){
        System.out.println("Gift card");
        //complete the code
        
        }
    }
}
```

### Logical Statements

Q. You're a tour manager and need a program that will identify small countries.
A country is considered small if its population is under 10000 and its area is under 10000 hectares.
The given program takes population and area as input.
 
Task
Complete the program to output "small country" if both conditions are met. Don't output anything otherwise.

Sample Input
9955
7522

Sample Output
small country


```

import java.util.Scanner;

public class Main {
   public static void main(String[] args) {
       Scanner read = new Scanner(System.in);
       int population = read.nextInt();
       int area = read.nextInt();
        //Complete the code
        if (population < 10000){
            if (area < 10000){
                System.out.println("small country");
            }
        }
   }
   
}

```

### 

Q. Your robot can recognize your emotions marked with number that represents each of them:
1 - You are happy!
2 - You are sad!
3 - You are angry!
4 - You are surprised!
Write a program that takes the emotion number as input and outputs the corresponding message in given format.
If the input is an emotion that the program doesn’t know, it should output: "Unknown emotion.".

Sample input
1
Sample output
You are happy!

```
import java.util.Scanner;

public class Main {
   public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);
       int emotion = scanner.nextInt();
       /*
       1 - "You are happy!"
       2 - "You are sad!"
       3 - "You are angry!"
       4 - "You are surprised!"
       other - "Unknown emotion."
       */
       
       // your code goes here
       
       switch (emotion){
           case 1:
            System.out.println("You are happy!");
           break;
           case 2:
            System.out.println("You are sad!");
           break;
           
           case 3:
            System.out.println("You are angry!");
           break;
           case 4 : 
            System.out.println("You are surprised!");
           
           break ;
           default: 
           System.out.println("Unknown emotion.");
           break ;
       }
       
   }
}
```

### while loops

Q. For your math class you need a program to calculate the factorial of a number.
You're given a program which takes a number as input. 

Task
Complete the program to calculate the factorial of the given number and output it.

Sample input
6

Sample output
720

Explanation
The factorial of a number is equal to the product of all  numbers less than or equal to the given number.
The factorial of 6 will be  6*5*4*3*2*1 = 720.

Hint
Use while loop to calculate the factorial of the number.

``` 

import java.util.Scanner;

public class Main
{
	public static void main(String[] args) {
	    Scanner scanner = new Scanner(System.in);
            int  number = scanner.nextInt();
            int fact = 1;
            //your code goes here
       
            while (number  > 0){
            fact *=number;
            number--;
                
            }
            System.out.println(fact );
    }
}

```

### 