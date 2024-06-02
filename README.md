using System;

class Program
{
    static void Main(string[] args)
    {
        Console.Write("Enter a numerical grade between 0 and 100: ");
        string input = Console.ReadLine();
        int grade;

        if (int.TryParse(input, out grade) && grade >= 0 && grade <= 100)
        {
            if (grade >= 90)
            {
                Console.WriteLine("A");
            }
            else if (grade >= 80)
            {
                Console.WriteLine("B");
            }
            else if (grade >= 70)
            {
                Console.WriteLine("C");
            }
            else if (grade >= 60)
            {
                Console.WriteLine("D");
            }
            else
            {
                Console.WriteLine("F");
            }
        }
        else
        {
            Console.WriteLine("Invalid input. Please enter a number between 0 and 100.");
        }
    }
}
