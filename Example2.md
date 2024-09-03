//This is our first C# program

using static System.Console;//no longer need WriteLine.Console now
//putting static means that you dont have to call the object
//if you dont put [.Console] then you dont need the static
//Console is a method/object --> static makes it so that it doesnt have to be created
    //if want code to run without creating object

public class HelloWorld{
    public static void Main(string[] args){
        
        //Init's(Initalizations)
        double someMoney = 39.45;
        double someNumber = 3.0;
        
        //Display the monetary value to the user
        WriteLine("The money is $");
        //dont need Console.WriteLine --> because console is imported, would be legacy code that breaks
        WriteLine("The money is ${0}. Can add things to end.",someMoney);
        //put brace around the index of the _____ you are going to display
        //0 is a placeholder, will be replaced with the value stored in the variable
        
        WriteLine("The number is {0}",someNumber);//use 0 as the placeholder
        
        WriteLine("The money is ${0}. Here is another number---> {1}, last number {2}",someMoney, 99.9, 21);
        //number are 0 based and referenced by the system accordingly
        //can change around the order of the variables that are printed based on the index number/ placeholders that are specified within the string argument
        
       //WriteLine--> will print out the values with a line in between
        WriteLine("{0}",4);
        WriteLine("{0}",56);
        WriteLine("{0}",789);
        
       
       //Write --> Will not print out the values with an line in between
        Write("{0}",4);
        Write("{0}",56);
        Write("{0}",789);
        //Output: 456789
        
      //Making Tables
       WriteLine("{0, 5}",4);//will right justify
       //if you want to left justify, then put a negative in front of the 5
         WriteLine("{0, -5}",4);//will left justify
         WriteLine("{0, -10}",4);//will left justify
        WriteLine("{0}",56);
        WriteLine("{0}",789);
        
        //Output Manipulation
         WriteLine("{0, -5}{1,10}{2,10}",4, "Nash", "Landon");
         //argument 2 is landon
         //argument 1 is Nash
         //argument 0 is 4
        
        ////////////////////////////////////////////////////////
        //Large Number/Value Notation
        int otherMoney = 123_456_789;
        //underscores have no effect on the value, increase readability
        WriteLine("The large number is {0}",otherMoney);
        

        
    }//End: Main
}//End: Class
