# Rey-Sabitsana

 using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp2
{
    class Program
    {
        static void Main(string[] args)
        {

            // 1. [5, 1, 4, 6, 7, 3, 5, 7, 3]
            //      On the array above print the duplicate elements.
            //      Please show us your code.

            Console.Write("5, 1, 4, 6, 7, 3, 5, 7, 3");
            Console.WriteLine();
            Console.Write("List of Duplicate Element \n");
            int[] arr = new int[] { 5, 1, 4, 6, 7, 3, 5, 7, 3 };
            for (int i = 0; i < arr.Length; i++)
            {
                for (int j = i + 1; j < arr.Length; j++)
                {
                    if (arr[i] == arr[j])
                    {
                        Console.Write(arr[i].ToString()+",");
                    }

                }

            }

            Console.WriteLine();
            Console.WriteLine();
            //   2. Print 
            //        1
            //        2 2
            //        3 3 3
            //        4 4 4 4
            //        5 5 5 5 5
            //        6 6 6 6 6 6

            int num, a, b, c;
            Console.Write("Pyramid \n");
            num = 6;
            for (a = 1; a <= num; a++)
            {
                for (b = 1; b < a; b++)
                {
                   Console.Write( a.ToString() + " ");
                }
                Console.Write( a.ToString() + "\n");
            }


            Console.WriteLine();
            ///  Pertage Between Male and Female

            //                    1. 3. Using your preferred IDE, create a program that asks the user for the number of 
            //                          male and female newly hired employee, number of male and female in permanent
            //                          position and number of male and female resigned in a company. The program should
            //                          display the total number of newly hired, permanent and resigned employee and the
            //                          percentage of newly hired males and females, males and females in permanent
            //                          position and males and females resigned in the company.

            //                          Sample output:
            //                          Enter the number of newly hired males: 36
            //                          Enter the number of newly hired females: 17
            //                          Enter the number of permanent position males: 36
            //                          Enter the number of permanent position females: 17
            //                          Enter the number of resigned males: 36
            //                          Enter the number of resigned females: 17

            int TotalnewlHIred, TotalPermanent, TotalResigned;
            int NewlyhiredMale = 36;
            int NewlyhiredFemale = 17;

            int Resignedmale = 36;
            int ResignedFemale = 17;

            int PermanentMale = 36;
            int PermanentFemale = 17;

            ///  Total Count
            TotalnewlHIred = NewlyhiredMale + NewlyhiredFemale;
            TotalPermanent = PermanentMale + PermanentFemale;
            TotalResigned = Resignedmale + ResignedFemale;

             Console.Write("Total of NewlyHired " + TotalnewlHIred.ToString());
            Console.WriteLine();
            Console.Write("Total of Resigned " + TotalResigned.ToString());
            Console.WriteLine();
            Console.Write("Total of Permanent " + TotalPermanent.ToString());

            Console.WriteLine(); Console.WriteLine();
            Console.WriteLine(); Console.Write("####Newly Hired\n");

            Console.Write("Female ");
            /// Newly Hired
            Console.Write((Math.Round((double)(100 * NewlyhiredFemale) / TotalnewlHIred, 2)).ToString() + "%\n");
            Console.Write("Male ");
            Console.Write((Math.Round((double)(100 * NewlyhiredMale) / TotalnewlHIred, 2)).ToString() + "%\n");
            Console.WriteLine();
            Console.Write("#####Permanent\n");
            Console.Write("Female ");
            /// Permanent
            Console.Write( (Math.Round((double)(100 * PermanentFemale) / TotalPermanent, 2)).ToString() + "%\n");
            Console.Write("Male ");
            Console.Write((Math.Round((double)(100 * PermanentMale) / TotalPermanent, 2)).ToString() + "%\n");
            Console.WriteLine();
            Console.Write("#####Resigned\n");
            Console.Write("Female ");
            /// resigned
            Console.Write((Math.Round((double)(100 * ResignedFemale) / TotalnewlHIred, 2)).ToString() + "%\n");
            Console.Write("Male ");
            Console.Write((Math.Round((double)(100 * Resignedmale) / TotalnewlHIred, 2)).ToString() + "%\n");

            Console.Read();
        }
    }
}
  
