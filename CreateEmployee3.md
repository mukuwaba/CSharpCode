using static System.Console;

class CreateEmployee3{
    
    static void Main(){
        
        Employee aWorker = new Employee();
        //Employee()--> blue print
        //aWorker--> variable name for the new instance of the object
        
        aWorker.IdNumber = 3872;
        aWorker.Salary = 22.11;
        
    }//Main
}//End: CreateEmployee3

//This is a blueprint for employee objects
class Employee{
    
    public int IdNumber(get; set;)
    public double Salary (get; set;)
    
}//End: Employee
