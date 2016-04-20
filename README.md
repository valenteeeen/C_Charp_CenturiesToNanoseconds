/*
C# CenturiesToMinutes
Write program to enter an integer number of centuries and convert it to years, days, hours and minutes
*/
using System;

class CenturiesToNanoseconds
{
    static void Main()
    {
        Console.Write("Centuries = ");
        int centuries = int.Parse(Console.ReadLine());
        int years = centuries * 100;
        ulong days = (ulong)(years * 365.2422);
        ulong hours = 24 * days;
        ulong minutes = 60 * hours;
        ulong seconds = 60 * minutes;
        ulong milliseconds = 1000 * seconds;
        ulong microseconds = 1000 * milliseconds;
        decimal nanoseconds = 1000M * microseconds;//(decimal)
        Console.WriteLine("{0} centuries = {1} years = {2} days = {3} hours = {4} minutes = {5} seconds = {6} miliseconds = {7} microseconds = {8} nanoseconds", centuries, years, days, hours, minutes,seconds, milliseconds, microseconds, nanoseconds);
    }
}

/*Console.WriteLine("{0} centuries = {1} years = {2} days = {3} hours = {4} minutes", centuries, years, days, hours, minutes);
*/
/*Centures = 5
5 centuries = 500 years = 182621 days = 4382904 hours = 262974240 minutes = 15778454400 seconds = 15,778,454,400,000 milliseconds = 15,778,454,400,000,000 microseconds = 15,778,454,400,000,000,000 nanoseconds
*/
