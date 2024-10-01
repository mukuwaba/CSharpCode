// Online C# Editor for free
// Write, Edit and Run your C# code using C# Online Compiler

using System;
using static System.Console;

public class RandomNumGen{
    public static void Main(string[] args){
        
    Random ranNumberGenerator = new Random();

    int randomNumber;

    randomNumber = ranNumberGenerator.Next(MIN, MAX);
        
    Console.WriteLine ("Enter an integer: ");
    pickedNum = ReadLine();
    pickedNum = Convert.ToInt32(numberString);
    
    if(pickedNum == randomNumber){
        WriteLine("congrats you have guessed the correct number");
    }//End: if
        
   
   
    }//End:main
}//End:class
