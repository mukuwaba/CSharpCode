// Online C# Editor for free
// Write, Edit and Run your C# code using C# Online Compiler

using System;
using static System.Console;

public class SortArray{
    public static void Main(string[] args){
        
        string[] names = {"Omar", "Patty", "Roger", "Tacker"};//intilization and declaration
       
        int x;//declaration only --> 
        //Declaration--> you exsist and this is your name
        //Initalization--> setting the variable equal to something
        WriteLine("_________________________________________________");
        WriteLine("Hey this is not sorted");
        for( x=0; x<names.Length; x++){
            
            WriteLine(names[x]);
            
        }
        WriteLine("_________________________________________________");
        Array.Sort(names);
        WriteLine("Hey this is sorted");
        for( x=0; x<names.Length; x++){
            
            WriteLine(names[x]);
            
        }
        
        WriteLine("_________________________________________________");
        Array.Reverse(names);
        WriteLine("Hey this is reversed");
        for( x=0; x<names.Length; x++){
            
            WriteLine(names[x]);
            
        }
        
        
    }//End: main
}//Emd: SortArray
