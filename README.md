
THIS IS CODED IN C# AND MADE IN VISUAL STUDIO BUT ANYTHING THAT RUNS .NET IN C# WILL WORK (also use the console not the terminal)












using System;

namespace login_or_register_system
{
    class Program
    {
        static void Main(string[] args)
        {
            // creats some string and some doubles
            string email = "your email here <-----";

            bool isRegistered;

            string userName = "hayden";

            string password = "2019";

            // asks if the user is registerd

            Console.WriteLine("HI, if you are already register type : yes, if you are not register type : no.");

            // creats a string that takes the users answer

            string userAnswer = Console.ReadLine();

            // compare if the user imputed yes or no

            if (userAnswer == "yes")
            {
                isRegistered = true;
            } else
            {
                isRegistered = false;
            }
            if (isRegistered == false)
            {
                // if the user is not registered this is the code

                // it sets the boolean to fallse on a default

                bool correctEmail = false;

                bool correctPassword = false;

                // asks to do the login procces

                Console.WriteLine("you are not loged in please enter your email press enter and then your password");

                // takes the user imformation to compare them

                string mail = Console.ReadLine();

                string password2 = Console.ReadLine();

                // compares it

                if (mail == email)
                {
                    correctEmail = true;
                }else
                {
                    Console.WriteLine("password or email is incorrect try reseting the solution");
                }
                if (password2 == password)
                {
                    correctPassword = true;
                }
                if (correctEmail == true && correctPassword == true)
                {
                    Console.WriteLine(userName + " is registered and loged into your account");
                }else  
                {
                    Console.WriteLine("password or email incorect try reseting the solution");
                }
            }

            if (isRegistered == true)
            {
                // login procces for the yes answer

                Console.WriteLine("cool, to log into your account enter your password...");

                var passwordAnswer = Console.ReadLine();

                if (passwordAnswer == password)
                {
                    Console.WriteLine("Cool you are loged in as the user " + userName);
                } else
                {
                    Console.WriteLine("your password is incorrect, try reseting the solution");
                }
                

                
                
                
                
                
                
                
            }

        }
    }
}
