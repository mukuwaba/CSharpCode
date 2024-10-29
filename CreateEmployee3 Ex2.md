
class CreateEmployee3{
    
    static void Main(){
        
        Employee aWorker = new Employee();
        //Employee()--> blue print
        //aWorker--> variable name for the new instance of the object
        
        aWorker.setIdNumber(3872);
        //pass through the set method
        
        
        aWorker.Salary = 22.11;
        
        System.Console.WriteLine("Employee #{0} makes ${1}", aWorker.getIdNumber(), aWorker.Salary.ToString());

    }//Main
}//End: CreateEmployee3

//This is a blueprint for employee objects
class Employee{
    
    //Mutator Method--> will change something (IdNumber)
    public void setIdNumber(int someValue){
        this.IdNumber = someValue;
        
    }//End:setIdNumber
    
    //Access Method
    public int getIdNumber(){
        return this.IdNumber;
    }//End:getIdNumber
    
    //instance variables
    private int IdNumber;
    public double Salary;
    //if IdNumber is private then the method above cannot access it.
    
}//End: Employee
