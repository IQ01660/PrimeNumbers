# PrimeNumbers

C#'''
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace PrimeNumbers
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter a number");
            string enteredString = Console.ReadLine(); // taking the input
            int enteredNum = Convert.ToInt32(enteredString); // converting input into number
            if (enteredNum > 0) // cheking if the number is positive
            {
                bool isPrime = true;
                for (int i = 2; i < enteredNum; i++) // checking all dividents before the input number
                {
                    if (enteredNum % i == 0)// cheking if the number is divisible by i
                    {
                        isPrime = false;
                    }
                }
                
                // giving the output
                if (isPrime == true)
                {
                    Console.WriteLine(enteredNum+" is a prime number");
                }
                else
                {
                    Console.WriteLine(enteredNum+" is NOT a prime number");
                }
            }
            else
            {
                Console.WriteLine("This is not a positive number");
            }
        }
    }
}

'''
