//This is an example of using a "switch" statement
using System;//!!!!!!!!!
using static System.Console;//incompatable with 4.8 and sooner

public class SwitchExample{
    public static void Main(string[] args){//where execution begins
    
    //Constants
    const int STOP = -1; //Flag to end execution
    const int IGNORE = 999; //Flag to ignore something
    
    //Inits
    int nYear = IGNORE; //Int to ignore selection
    //nYear--> prefix the variable name with the data type
    //  n--> integer
    //  Hungarian notation
    
    //do--> like while loop but executes body of the code first
    //A "do" loop gunartees execution of the loop body at least once
    
    //Start looping
    do{
        //Determine selection based on year
        switch(nYear){
            
            case IGNORE:
                WriteLine("We're ignoring...");
                break;
            
            case 0:
                //WriteLine("We hit a 0 or a 1.");
                //intentionally leaving out the break
           
            case 1:
                WriteLine("We hit a 0 or a 1.");
                break;
                
            case 2:
                WriteLine("You typed the number \"2\"");
                break;
             
            case 3:
                WriteLine("3");
                break;
            
             case 4:
                WriteLine("4");
                break;
            
            default:
                WriteLine("Default was encountered");
                break;
                //incase none of the other conditions apply
                //use defaults as error traps
            
        }//End; switch
        
        //Prompt the User
    Write("Enter a year (-1 stops execution): ");
       nYear = Convert.ToInt32(ReadLine());
        //ReadLine --> gets input from the user
        
    }//End: do
    
    while(nYear != STOP);//Loop var check
        
    WriteLine("We're all done! Ending the program!");
    
    
    //!= --> NOT
    //(nYear != STOP)--> Loop variable check
    //without break execution will fall into the next case,
    //only should be used in switch statements
        
    }//End: main
}//End:class
