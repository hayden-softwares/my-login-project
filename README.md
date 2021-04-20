using System;

namespace login_system_2
{
    class Program
    {

        public static string userName;
        public static string password;

        static void Main(string[] args)
        {
            Console.WriteLine(" login youre browser account, Insert the user name");
            userName = Console.ReadLine();
            Console.WriteLine("Enter the password");
            password = Console.ReadLine();
            Register();
            Login();

        }

        public static void Register()
        {
            Console.WriteLine("enter the user name");
            userName = Console.ReadLine();
            Console.WriteLine("Enter the password");
            password = Console.ReadLine();
            if (userName == userName)
            {
                Console.WriteLine("register completed now login into youre account");
            }
            else
            {
                Console.WriteLine("register failed try restarting the program");
            }
        }

        public static void Login()
        {
            Console.WriteLine("enter the user name");
            userName = Console.ReadLine();
            Console.WriteLine("Enter the password");
            password = Console.ReadLine();
            if (userName == userName)
            {
                Console.WriteLine("login completed");
            }
            else
            {
                Console.WriteLine("login failed try restarting the program");


            }

        }
    }
}

