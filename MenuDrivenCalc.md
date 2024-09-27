//Note to Professor: When using the online compiler (programiz.com) sometimes an error occurs when entering certain numbers as numberAsString_1 via user input. As far as I can tell there is nothing within the code that would generate this error. However, the only number that errors on my end is the number 5. All other numbers seem to work fine. 

using System;
using static System.Console;

public class MenuDrivenCalc{
    public static void Main(string[] args) {
        
        //Inits
         string    numberAsString_1;
         string    numberAsString_2;
         string    operationAsString;
         int       numberAsInt_1;
         int       numberAsInt_2;
         int       answer;
         int       operationAsInt;
        
  
        
        //Prompt the User
        WriteLine("Please enter the first number: ");
        numberAsString_1 = ReadLine();
        numberAsInt_1 = Convert.ToInt32(numberAsString_1);
        
        WriteLine("Please enter the second number: ");
        numberAsString_2 = ReadLine();
        numberAsInt_2 = Convert.ToInt32(numberAsString_2);
        
        //Insert space for cleaner interface
        WriteLine("");
        WriteLine("");
        
        WriteLine("Operations");
        WriteLine("1. Addition");
        WriteLine("2. Subtraction");
        WriteLine("3. Division");
        WriteLine("4. Multiplication");
        
        //Insert space for cleaner interface
        WriteLine("");
        WriteLine("");
        
        WriteLine("Enter the number of the desired operation: ");
        operationAsString = ReadLine();
        operationAsInt= Convert.ToInt32(operationAsString);
        
        //Insert space for cleaner interface
        WriteLine("");
        WriteLine("");
        
        //Switch Statement
        switch(operationAsInt){
            case 1:
                answer = numberAsInt_1 + numberAsInt_2;
                WriteLine("Answer: " +answer);
                break;
            case 2:
                answer = numberAsInt_1 - numberAsInt_2;
                WriteLine("Answer: " +answer);
                break;
            case 3:
                answer = numberAsInt_1 / numberAsInt_2;
                WriteLine("Answer: " +answer);
                break;
            case 4:
                answer = numberAsInt_1 * numberAsInt_2;
                WriteLine("Answer: " +answer);
                break;
            default:
                WriteLine("Please enter a number corresponding to the given operations. Re-run program to try again. ");
                        WriteLine("Operations");
                        WriteLine("1. Addition");
                        WriteLine("2. Subtraction");
                        WriteLine("3. Division");
                        WriteLine("4. Multiplication");
                        break;
            
        }//End: switch
        
    WriteLine("Thank you for using the Menu Driven Calculator. Please re-run program to perform another calculation.");
    
        
    }//End: main
}//End:class

//References
//pg.68 --> prompt user, conversions
//pg. 128 --> using switch statements
//pg. 49 --> using Arithmatic Operators
