# Assignment
int count = 0;
    
               Console.Write("Enter first num: ");
               int m = Int32.Parse(Console.ReadLine());
               Console.Write("Enter second num: ");
               int n = Int32.Parse(Console.ReadLine());
    
               for (int i = m; i <= n; i++)
               {
                    if (i % 5 == 0) count++;
               }
    
               Console.WriteLine("{0} numbers found.", count);

               //  No 2

               
               int number1 = 0;
               int number2 = 1;
               int sum = 1;
               int counter = 0;
    
               Console.WriteLine(number1);
    
               while(counter < 100)
               {
                    sum = number1 + number2;
                    number1 = number2;
                    number2 = sum;
                    Console.WriteLine(number2);
                    counter++;

               }

                                       //  No 3
               
               
               
               Console.Write("Enter first number: ");
               int v = Int32.Parse(Console.ReadLine());
               Console.Write("Enter second number: ");
               int w = Int32.Parse(Console.ReadLine());
               Console.Write("Enter third number: ");
               int x = Int32.Parse(Console.ReadLine());
               Console.Write("Enter fourth number: ");
               int y = Int32.Parse(Console.ReadLine());
               Console.Write("Enter fifth number: ");
               int z = Int32.Parse(Console.ReadLine());
    
               if (v < w) v = w;
               if (v < x) v = x;
               if (v < y) v = y;
               if (v < z) v = z;
                Console.WriteLine("{0} is the biggest number.", v);
                    // No 4

               Console.Write("Input A (not 0): ");
               sbyte a = Convert.ToSByte(Console.ReadLine());
               Console.Write("Input B: ");
               sbyte b = Convert.ToSByte(Console.ReadLine());
               Console.Write("Input C: ");
               sbyte c = Convert.ToSByte(Console.ReadLine());

               sbyte d = (sbyte)(b * b - 4 * a * c);
               if (d < 0)
                 Console.WriteLine("\nD={0}\nThere are no real roots.", d);
               else if (d == 0)
               {
                  sbyte x1 = (sbyte)(-b / 2 * a);
                  Console.WriteLine("\nX={0}", x1);
               }
               else
               {
                  sbyte x1 = (sbyte)((-b + Math.Sqrt(d)) / (2 * a));
                  sbyte x2 = (sbyte)((-b - Math.Sqrt(d)) / (2 * a));
                  Console.WriteLine("\nX1={0}\nX2={1}", x1, x2);
               }
               Console.ReadLine();
            
               
         
               
               
               
                            // No 5
                           
              byte points;
             Console.Write("Enter points between 1 and 9: ");
             points = Convert.ToByte(Console.ReadLine());
             if (points >= 1 && points <= 3)
                Console.WriteLine("Points multiplied by 10: {0}", points * 10);
             else if (points >= 4 && points <= 6)
                Console.WriteLine("Points multiplied by 100: {0}", points * 100);
             else if (points >= 7 && points <= 9)
                Console.WriteLine("Points multiplied by 1000: {0}", points * 1000);
             else
                Console.WriteLine("Wrong Input!");
             Console.ReadLine();
                // NO 6

               
             Console.Write("Enter N: ");
             int length = Int32.Parse(Console.ReadLine());

             for (int i = 1; i < length; i++)
             {
                 if (i % (3 * 7) != 0) Console.WriteLine(i);
             }

                      // No 7

             

             for (int i = 0; i < 4; i++)
            {
                if(i != 0) Console.WriteLine();

                for (int j = 0; j < 13; j++)
                {
                    switch (i)
                    {
                        case 0: Console.Write("Hearts "); break;
                        case 1: Console.Write("Diamonds "); break;
                        case 2: Console.Write("Spades "); break;
                        case 3: Console.Write("Clubs "); break;
                    }
                    switch(j)
                    {
                        case 0: Console.WriteLine("2"); break;
                        case 1: Console.WriteLine("3"); break;
                        case 2: Console.WriteLine("4"); break;
                        case 3: Console.WriteLine("5"); break;
                        case 4: Console.WriteLine("6"); break;
                        case 5: Console.WriteLine("7"); break;
                        case 6: Console.WriteLine("8"); break;
                        case 7: Console.WriteLine("9"); break;
                        case 8: Console.WriteLine("10"); break;
                        case 9: Console.WriteLine("J"); break;
                        case 10: Console.WriteLine("Q"); break;
                        case 11: Console.WriteLine("K"); break;
                        case 12: Console.WriteLine("A"); break;
                    }
                }
            }
            Console.ReadLine();
            //      No 10
            
            

            int[] arr = new int[20];

            for (int i = 0; i < arr.Length; i++)
            {
                arr[i] = i * 5;
                Console.WriteLine(arr[i]);
            }
                               // 12
               

             int Count = 1, tempCount = 1, number = 0;

			    Console.Write ("Enter array length: ");
			    int Length = Int32.Parse (Console.ReadLine ());
			    int[] Array = new int[length];

             for (int i = 0; i < Array.Length; i++) 
			   {
				    Console.Write ("Enter {0} element: ", i);
				    Array [i] = Int32.Parse (Console.ReadLine ());
			   }

			   for (int i = 0; i < Array.Length - 1; i++) 
			   {
                  if (arr[i] == Array[i + 1]) tempCount++;
                  else tempCount = 1;

				  if (tempCount > Count) 
				{
					Count = tempCount;
					number = Array [i];
				}
			   }

			     for (int i = 0; i < Count; i++) Console.Write ("{0}, ", number);
