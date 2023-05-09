using System;

class Program {
    static void Main (string[] args) {
        Console.Write("Enter your name:");
        string? name = Console.ReadLine();

        Console.Write("Enter your age:");
        int age = int.Parse(Console.ReadLine());

        string greeting = "";
        if (TwelveOrLess(age)) {
            greeting = "Hi, " + name + "! Stay in school.";
        } else {
            greeting = $"Hello, {name}! Nice to meet you.";
        }
        Console.WriteLine(greeting);

        int Months = age * 12;
        Console.WriteLine($"You are {Months} months old.");
    }
    static bool TwelveOrLess(int age) {
        return age < 12;
    }
}
