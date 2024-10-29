
class CreateEmployee3{
    
    static void Main(){
        
        Employee aWorker = new Employee();
        //Employee()--> blueprint
        //aWorker--> variable name for the new instance of the object
        
        aWorker.IdNumber= 3872;
        //pass through the set method
        
        
        aWorker.Salary = 22.11;
        
        System.Console.WriteLine("Employee #{0} makes ${1}", aWorker.IdNumber, aWorker.Salary.ToString());
        //need to call a method, use () and the get method

    }//Main
}//End: CreateEmployee3

//This is a blueprint for employee objects
class Employee{
    
    
    //instance variables
    public int IdNumber {get; set;}
    //tells the complier to create set and gets
    //shorthand method for set and get methods
    public double Salary;
    //if IdNumber is private then the method above cannot access it.
    
}//End: Employee
