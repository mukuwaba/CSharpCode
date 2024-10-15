//This will demo classes v. objects
using System;

public class DogHouseExample{
    public static void Main(string[] args){
        
        
        Console.WriteLine ("We're about to \"build\" a doghouse from a blueprint");
        
        
    }//End: main
}//End DogHouseExample

public class DogHouseBlueprint{
    
    string   name   = ""//Name of the dog
    string   color  = "white";
    int      weight = 10;//lbs
    
    //Mutator Methods
    //Mutator means that you're changing an attribute
    //set and get methods
    
    public void setName(string newName){
        
    this.name = newName;
        
    }//End: setName
    
    public void setColor(string newColor){
    
    this.color = newColor;
    
    ////////////////////////////////////////////
    //Access methods
    //bring values from the returm variables
    
    }//End setColor
    
    
    public string getName(){
        
        return this.name;
        
    }//end getName
    public string getColor(){
        
        return this.color;
        
    }//end getName
    
}//End: DogHouseBlueprint
