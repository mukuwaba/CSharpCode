//This will demo classes v. objects
using System;

public class DogHouseExample{
    public static void Main(string[] args){
        
        
        Console.WriteLine ("We're about to \"build\" a doghouse from a blueprint");
        
        DogHouseBlueprint myFirstDogHouse = new DogHouseBlueprint();
        //have to give the new object a type = myFirstDogHouse
        //a reference to the thing you create
        
        myFirstDogHouse.setName("Toddy");
        
        myFirstDogHouse.setColor("Red");
        
        Console.WriteLine(myFirstDogHouse.getColor());
        //myFirstDogHouse is the variable name
        //getColor is a method | defaulted to white
        
        Console.WriteLine(myFirstDogHouse.getName());
        //need () because it is a method call that will return information
        
        DogHouseBlueprint mySecondDoghouse = new DogHouseBlueprint();
        //mySecondDoghouse is a different object but still from the same class and blueprint
        Console.WriteLine(mySecondDoghouse.getColor());
        mySecondDoghouse.setName("Spot");
        mySecondDoghouse.setColor("Black and White");
        
        Console.WriteLine(mySecondDoghouse.getName());
        Console.WriteLine(mySecondDoghouse.getColor());
        
       
        

        
        
    }//End: main
}//End DogHouseExample

public class DogHouseBlueprint{
    //tells the complier how to 'build' something
    
    string   name   = "";//Name of the dog
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
