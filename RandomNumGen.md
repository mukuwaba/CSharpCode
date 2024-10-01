// Online C# Editor for free
// Write, Edit and Run your C# code using C# Online Compiler

using System;
using static System.Console;

public class RandomNumGen{
    public static void Main(string[] args){
            
        //Inits
        int randomNumber;
        
        string pickedNum;
        
        int pickedNumAsInt;
        
        //Generate Random Number
        Random ranNumberGenerator = new Random();
        
        randomNumber = ranNumberGenerator.Next(1,10);
        
        
        //Test Code --> reveals value of randomNumber
        //WriteLine(""+randomNumber);
         
            
        //Prompt user for input
        Console.WriteLine ("Enter an integer: ");
        pickedNum = ReadLine();
        pickedNumAsInt = Convert.ToInt32(pickedNum);
        
        //Determine whether correct number was entered
        if(pickedNumAsInt == randomNumber){
            WriteLine("Congratulations!!! You have guessed the correct number!");
            
        }//End: if
        
        else{
            WriteLine("The number you have entered is incorrect. Please Try Again.");
        }//End: else
    }//End:main
}//End:class
