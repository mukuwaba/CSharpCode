
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        List<string> userInputList = new List<string>();
        string input;
        
        Console.WriteLine("Enter your inputs (type 'exit' to stop):");
        
        while (true)
        {
            input = Console.ReadLine();
            if (input.ToLower() == "exit")
                break;
            userInputList.Add(input);
        }
        
        Console.WriteLine("You have entered the following inputs:");
        foreach (string item in userInputList)
        {
            Console.WriteLine(item);
        }
    }
}
