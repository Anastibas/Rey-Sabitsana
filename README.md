# Rey-Sabitsana

  // 1. [5, 1, 4, 6, 7, 3, 5, 7, 3]
            //      On the array above print the duplicate elements.
            //      Please show us your code.

            label1.Text = "";
            label2.Text = "";
            int[] arr = new int[] { 5, 1, 4, 6, 7, 3, 5, 7, 3 };
            for (int i = 0; i < arr.Length; i++)
            {
                for (int j = i + 1; j < arr.Length; j++)
                {
                    if (arr[i] == arr[j])
                    {
                        if (label1.Text == "") { label1.Text += arr[i].ToString(); } else { label1.Text += ","+arr[i].ToString(); }
                    }
                }
            }

            //   2. Print 
            //        1
            //        2 2
            //        3 3 3
            //        4 4 4 4
            //        5 5 5 5 5
            //        6 6 6 6 6 6

            int num,a,b,c;

            num = 6;
            for (a = 1; a <= num; a++)
            {
                for (b = 1; b <a; b++)
                {
                    label2.Text += a.ToString()+" ";                 
                }
                label2.Text += a.ToString() + "\n";
            }


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

            ///  Total Count
            TotalnewlHIred = Convert.ToInt16(new3.Text) + Convert.ToInt16(new2.Text);
            TotalPermanent = Convert.ToInt16(per2.Text) + Convert.ToInt16(per3.Text);
            TotalResigned = Convert.ToInt16(res2.Text) + Convert.ToInt16(res3.Text);

            new1.Text =TotalnewlHIred.ToString();
            res1.Text = TotalResigned.ToString();
            Per1.Text = TotalPermanent.ToString();

            /// Newly Hired
            newper1.Text = (Math.Round((double)(100 * Convert.ToInt16(new2.Text)) / TotalnewlHIred,2)).ToString()+"%";
            newper2.Text = (Math.Round((double)(100 * Convert.ToInt16(new3.Text)) / TotalnewlHIred,2)).ToString()+"%";

            /// Permanent
            perper1.Text = (Math.Round((double)(100 * Convert.ToInt16(per2.Text)) / TotalPermanent, 2)).ToString()+"%";
            perper2.Text = (Math.Round((double)(100 * Convert.ToInt16(per3.Text)) / TotalPermanent, 2)).ToString()+"%";

            /// resigned
            resper1.Text = (Math.Round((double)(100 * Convert.ToInt16(res2.Text)) / TotalnewlHIred,2)).ToString()+"%";
            resper2.Text = (Math.Round((double)(100 * Convert.ToInt16(res3.Text)) / TotalnewlHIred,2)).ToString()+"%";
