# README
using System;

namespace MyPassions
{
    class Program
    {
        static void Main(string[] args)
        {
            // Declaration of my passions
            string[] passions = { "Programming", "Helping others", "Hardware" };

            Console.WriteLine("Welcome to my world!\n");
            Console.WriteLine("Here are my passions:\n");

            foreach (string passion in passions)
            {
                Console.WriteLine($"- {passion}");
            }

            Console.WriteLine("\nA little more about each of them:");

            // Display details about each passion
            SharePassion("Programming", "I love creating applications and solving complex problems with code.");
            SharePassion("Helping others", "I enjoy assisting others, whether through mentoring or problem-solving.");
            SharePassion("Hardware", "I'm passionate about computer hardware, building PCs, and learning about the latest tech.");

            // Add YouTube channel
            Console.WriteLine("\nI also share content on my YouTube channel. Come check out my videos!");
            Console.WriteLine("YouTube Channel: https://youtube.com/@swax");

            Console.WriteLine("\nFeel free to reach out if we share similar interests!");
        }

        static void SharePassion(string passion, string description)
        {
            Console.WriteLine($"\n{passion}:\n{description}");
        }
    }
}
