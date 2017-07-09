# Beverage-Labels
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Beverage_Labels
{
    class Program
    {
        static void Main(string[] args)
        {
            string name = Console.ReadLine();
            int volume = int.Parse(Console.ReadLine());
            int energy = int.Parse(Console.ReadLine());
            int sugar = int.Parse(Console.ReadLine());

            double vol = volume / 100.00;
            double kcalEnergy = vol * energy;
            double sugars = vol * sugar;

            Console.WriteLine($"{volume}ml {name}:");
            Console.WriteLine($"{kcalEnergy}kcal, {sugars}g sugars");
        }
    }
}
