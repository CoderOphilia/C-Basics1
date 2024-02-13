using System;
namespace Text
{
    class Program
    {
        static void Main(string[] args)
        {
            //C# characters
            char c = 'a';
            char d = '1'; //it take 2 bytes of memory [16 bit]
            int i = sizeof(char);
            Console.WriteLine(i);

            //C# strings
            string s = "Hello"; //string memory is not defined

            //Diffrent ways to represent strings
            //1. Literals
            string str1 = "World";
            //2. Verbatim
            string str2 = @"c:\myfolder\newProgram.txt"; //here there is an escape sequence, but when we use @ infront of the string it makes the whole string into one. This is called as verbatim
            //3. Interpolated
            string str3 = $"Hello {str1}";
            Console.WriteLine(str3);

            Console.Write("Enter Your Name:");
            string name = Console.ReadLine();
            Console.WriteLine($"Hello {name}!!");

            //Unary Operator
            //1. increment operator 
            int a = 10;
            int b = a++;// b = a then a will become a+1, b= 10 , a =11
            int c1 = 10;
            int d1 = --c1; // d = 9 , c = 9
            Console.WriteLine($"{a},{b},{c1},{d1}");

            //assignment operator 
            //1. a+=b
            //2. a-=b
            //3. a*=b
            //4. a/=b
            //5. a=b

            //Comparison Operator
            //1. ==
            //2. !=
            //3. >
            //4. <

            //Conditional Operators
            //1. && (AND)
            //2. OR (OR)

            //Bitwise Operators
            //1. & (AND) //assume a = 1, b = 0 so a&b is interpreted as 1 if both are 1, otherwise 0. c= (a & b) , c = 0
            //2. | (OR) //1 if either of the value is 1, c = (a | b) , c = 1
            //3. ^ (XOR) // 0 if both are 1 or 0, otherwise 1 , c = a^b, c = 1


            Console.ReadKey();


        }
    }
}
