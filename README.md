using System;

namespace HelloApp
{
    class Program
    {
        static void Main(string[] args)
        {
            while (true)
            {
                double num1, num2;
                string anum1, anum2;
                Console.WriteLine("Введите два числа в диапазоне от 0 до 10");
                anum1 = Console.ReadLine();
                bool res1 = double.TryParse(anum1, out num1);
                anum2 = Console.ReadLine();
                bool res2 = double.TryParse(anum2, out num2);
                if (res1 && res2 == true)
                {
                    if (num1 >= 0 && num1 <= 10 && num2 >= 0 && num2 <= 10 == true)
                    {
                        Console.WriteLine("Вот произведение двух чисел = " + num1 * num2);
                        break;
                    }
                    else
                    {
                        Console.WriteLine("Числа введенны неверно попробуйте повторить");
                    }
                }
                else
                {
                    Console.WriteLine("Числа введенны неверно попробуйте повторить");
                }


                }

            }
        }
    }
