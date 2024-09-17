using System;
using static System.Console;
//static--> dont have to create an instance of the class, can refference method within the class
//will reference a console

public class HelloWorld{
    //public is an 'access modifier', tells what has access to the class
    //public --> open for all
   public static void Main(string[] args){
       //static--> can run main without creating any objects
       //void--> returning nothing
       
       //Inits
       const int HIGH = 10;//this is the largest value...
       //const --> constant, means that the value cannot change
       //int--> the (data) type of the constant is integer
       
       string    numberString;//not initalized
       
       int       number;//not initalized
       
       
      Write("Enter an Integer: ");//Prompt the user
      
      numberString = ReadLine();//Get the value from user
      //assignment statement
      //ReadLine() part of System suite
      
      //TYPE Casting
      //convert user input into integer
      number = Convert.ToInt32(numberString);
      //convert the string to a 32 bit integer
      
      
      //Validating the input number
      if(number > HIGH){
          WriteLine("{0} is greater than {1}",number, HIGH);
          //0 and 1 are indexes, placeholders for values
          //can also input numeric values to replace the placeholders at the end of the line, before the end of the parenthesis
      }//End: if
      
      else{
          WriteLine("{0} is not greater than {1}",number, HIGH);
      }//End: else
      
   
    }//End: main
}//End: Class
