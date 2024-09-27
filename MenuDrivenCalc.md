using System;
using static System.Console;

public class MenuDrivenCalc{
    public static void Main(string[] args) {
        
        //Inits
         string numberAsString_1;
         string numberAsString_2;
         string operationAsString;
         int numberAsInt_1;
         int numberAsInt_2;
         int answer;
  
        
        //Prompt the User
        WriteLine("Please enter the first number: ");
        numberAsString_1 = ReadLine();
        numberAsInt_1 = Convert.ToInt32(numberAsString_1);
        WriteLine("Please enter the second number: ");
        numberAsString_2 = ReadLine();
        numberAsInt_2 = Convert.ToInt32(numberAsString_2);
        
        WriteLine("Operations");
        WriteLine("1. Addition");
        WriteLine("2. Subtraction");
        WriteLine("3. Division");
        WriteLine("4. Multiplication");
        
        WriteLine("Enter the number of the desired operation: ");
        operationAsString = ReadLine();
    
        
        
        
    }//End: main
}//End:class

//References
//pg.68 --> prompt user, conversions
