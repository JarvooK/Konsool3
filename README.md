# Konsool3
Video 14:
using System;

namespace Konsool3
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Please enter your target?");
            int UserTarget = int.Parse(Console.ReadLine());

            int Start = 0; 

            while (Start <= UserTarget)
            {
                Console.Write(Start + " ");
                Start = Start + 2;    
            }
            string UserChoice = "";
            do
            {
                Console.WriteLine("do you want to continue - Yes or No?");
                UserChoice = Console.ReadLine().ToUpper();
                if (UserChoice != "YES" && UserChoice != "NO")
                {
                    Console.WriteLine("invalid Choice, Please say Yes or No");
                }
                while (UserChoice != "Yes" && UserChoice != "No") ;
            } while (UserChoice == "Yes");
            
            } 
    }
}
Video 15:
using System;

namespace Konsool3
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] numbers = new int[3];

            numbers[0] = 101;
            numbers[1] = 102;
            numbers[2] = 103;


            for(int j = 0; j < numbers.Length; j++)

            {
                Console.WriteLine(numbers[j]);
            }

            int i = 0;
            while(i < numbers.Length)
            {
                Console.WriteLine(numbers[i]);
                i++;
            }
        } 
    }
}
Video 16:
using System;

namespace Konsool3

{
    class Program
    {
        public static void Main()
        {
            Program.EvenNumbers(30);
            Program P = new Program();
           int Sum = P.add(10, 20);

            Console.WriteLine("Sum = {0}", Sum);
        }

        public int add(int FN, int SN)
        {
            return FN + SN;
        }

        public static void EvenNumbers(int Target)
        {
            int start = 0;
            while (start <= Target)
            {
                Console.WriteLine(start);
                start = start + 1;
            }

        }
    }
}
video 17:
using System;

namespace Konsool3
{
    class Program

    {
        public static void Main()
        {
            int Total = 0;
            int Produckt = 0;
            Calculate(10, 20, out Total, out Produckt);
            Console.WriteLine(" Sum = {0} && Produckt = {1}", Total, Produckt);
        }


        public static void Calculate(int FN, int SN, out int Sum, out int Produckt)
        {
            Sum = FN + SN;
            Produckt = FN * SN;
        }
    }
}

