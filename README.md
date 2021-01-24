using System;

namespace Basic_programs_2
{
    class Program
    {
        static void withoutspace(int num)
        {
            for(int i=1;i<=3;i++)
            {
                Console.Write(num);
            }
        }
        static void withspace(int num)
        {
            /*int rem, count;
            while(num>0)
            {
                rem %= 10;
                count++;
            }*/
            for(int i=1;i<=3;i++)
            {
                if (i != 2)
                    Console.Write(num);
                else
                {
                    //foreach (string j in count)
                    //{
                        Console.Write(" ");
                    //}
                }
            }
        }
        static void Main(string[] arg)
        {
            Console.Write("Enter the number: ");
            int num = Convert.ToInt32(Console.ReadLine());
            for(int i=1;i<=5;i++)
            {
                if(i==1 || i==5)
                {
                    withoutspace(num);
                    Console.WriteLine();
                }
                else
                {
                    withspace(num);
                    Console.WriteLine();
                }
            }
        }
    }
}
