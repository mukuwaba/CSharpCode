
class CreateEmployee3{
    
    static void Main(){
        
        Employee aWorker = new Employee();
        //Employee()--> blue print
        //aWorker--> variable name for the new instance of the object
        
        aWorker.IdNumber = 3872;
        aWorker.Salary = 22.11;
        
        System.Console.WriteLine("Employee #{0} makes {1}", aWorker.IdNumber, aWorker.Salary.ToString("C"));
        

    }//Main
}//End: CreateEmployee3

//This is a blueprint for employee objects
class Employee{
    
    //instance variables
    public int IdNumber;
    public double Salary;
    
}//End: Employee
