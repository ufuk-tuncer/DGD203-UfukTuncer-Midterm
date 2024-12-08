using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Dgd203_UfukTuncer_Midterm
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Welcome to the Game!");

            // Step 1: Get the player's name
            Console.Write("What is your name? ");
            string playerName = Console.ReadLine();
            Console.WriteLine($"Hello, {playerName}! Let's start the game!\n");

            // Questions and answers
            Console.WriteLine("Question 1: What is your favorite type of environment?");
            Console.WriteLine("  1. Mountains\n  2. Beach\n  3. Forest");
            string q1Answer = Console.ReadLine();

            Console.WriteLine("\nQuestion 2: What is your ideal way to spend a weekend?");
            Console.WriteLine("  a. Adventuring\n  b. Relaxing\n  c. Exploring new ideas");
            string q2Answer = Console.ReadLine();

            Console.WriteLine("\nQuestion 3: Choose your spirit animal:");
            Console.WriteLine("  1. Eagle\n  2. Dolphin\n  3. Wolf");
            string q3Answer = Console.ReadLine();

            Console.WriteLine("\nQuestion 4: Pick a superpower:");
            Console.WriteLine("  a. Flying\n  b. Telepathy\n  c. Super Strength");
            string q4Answer = Console.ReadLine();

            Console.WriteLine("\nQuestion 5: What's your favorite time of the day?");
            Console.WriteLine("  1. Morning\n  2. Afternoon\n  3. Night");
            string q5Answer = Console.ReadLine();

            Console.WriteLine("\nQuestion 6: What's your dream vacation?");
            Console.WriteLine("  a. A serene retreat\n  b. A bustling city adventure\n  c. A deep jungle exploration");
            string q6Answer = Console.ReadLine();

            // Step 4: Generate a remark based on the answers
            Console.WriteLine("\nCalculating your result...");

            string remark;

            if (q1Answer == "1" && q3Answer == "3")
            {
                remark = $"You are a true adventurer, {playerName}! You seek the untamed wilderness.";
            }
            else if (q2Answer == "b" && q4Answer == "b")
            {
                remark = $"Relaxed and intuitive, {playerName}, your inner peace draws people to you.";
            }
            else if (q5Answer == "3" && q6Answer == "c")
            {
                remark = $"Nighttime explorer, {playerName}! You are drawn to the mysteries of the unknown.";
            }
            else
            {
                remark = $"You are a unique individual, {playerName}, with a mix of strengths and dreams!";
            }

            Console.WriteLine(remark);
            Console.WriteLine("\nThanks for playing!");
        }
    
    }
}
