using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Threading;
using System.Diagnostics;

/// <summary>
/// Crackeur de mots de passe Multi-Threadé
/// Julien Ferluc
/// 2016-10-08
/// </summary>

namespace MultiThreadTest
{
    class Program
    {

        //Initializing some global variables (do not put variables that need to be accessed very often here because it will
        //probably slow down the program and render it somewhat unstable

        static long count;
        static string _crack;
        static string _password;
        static int _debut;
        static int _fin;
        static bool fini = false;

        static void Main()
        {
            //start message and setup of password
            Console.ForegroundColor = ConsoleColor.White;
            Console.WriteLine("Program initialized");
            Console.WriteLine("Reference: http://web.cs.du.edu/~mitchell/forensics/information/pass_crack.html");
            Console.WriteLine("");
            Console.WriteLine("What is the password to guess?");
            _password = Console.ReadLine();
            int passLength = _password.Length;

            Console.Clear();
            Console.WriteLine("What method would you like to use?");
            Console.WriteLine("random -> Proceed by randomly generating passwords and try them one by one");
            Console.WriteLine("file -> *EXPERIMENTAL* Use the content of a file containing passwords and try them one by one");
            string method = Console.ReadLine();

            Console.Clear();

            var stopwatch = new Stopwatch();

            switch (method)
            {
                case "random":

                    //min
                    Console.WriteLine("Minimum number of letters? (Example: if word = 4 letters then this would be 4; if lenght of word is unknow we suggest 3 minimum)");
                    _debut = int.Parse(Console.ReadLine());
                    Console.Clear();

                    //max
                    Console.WriteLine("Maximum number of letters?");
                    _fin = int.Parse(Console.ReadLine());
                    _fin = _fin + 1;
                    Console.Clear();

                    double time = Math.Round((Math.Pow(26, passLength) / 4000), MidpointRounding.AwayFromZero);

                    //PID
                    int nProcessID = Process.GetCurrentProcess().Id;
                    Console.Write(("pid: " + nProcessID));

                    //Date
                    Console.WriteLine(" Start time: " + DateTime.Now);

                    Console.WriteLine("Password lenght = " + passLength);
                    Console.WriteLine("Estimated tries: " + Math.Pow(26, passLength) + " -> " + time + "ms @ 4000t/ms");

                    Thread worker1 = new Thread(new ThreadStart(Worker1));
                    Thread worker2 = new Thread(new ThreadStart(Worker2));
                    //Thread worker3 = new Thread(new ThreadStart(Worker3));
                    //Thread worker4 = new Thread(new ThreadStart(Worker4));

                    worker1.Start();
                    worker2.Start();
                    //worker3.Start();
                    //worker4.Start();

                    //Starting stopwatch
                    stopwatch.Start();

                    //Post verification algorithm
                    while (true)
                    {
                        if (fini == true)
                        {
                            //Arret du timer et conversion du temps en millisecondes
                            stopwatch.Stop();
                            var elapsed = stopwatch.ElapsedMilliseconds;

                            //Stats et affichage du mot de passe
                            Console.ForegroundColor = ConsoleColor.Green;
                            Console.WriteLine("password: " + _crack);
                            Console.ForegroundColor = ConsoleColor.White;
                            if (count > 1000)
                            {
                                Console.WriteLine(count + " tries in " + elapsed + "ms @ " + count / elapsed + "t/ms");
                            }
                            else if (count > 1000)
                            {
                                Console.WriteLine("Error: Some threads couldn't initialize in time.");
                            }
                            break;
                        }
                    }
                    Console.Read();
                    break;

                case "file":
                    Console.WriteLine("What is the path of the password file you want to use? (ex: 'C:/Users/Username/Desktop')");
                    string filePath = Console.ReadLine();
                    string[] lignes = System.IO.File.ReadAllLines(filePath);
                    string password = _password;

                    //Starting stopwatch
                    stopwatch.Start();

                    foreach (string line in lignes)
                    {
                        if (password == line)
                        {
                            //Arret du timer et conversion du temps en millisecondes
                            stopwatch.Stop();
                            var elapsed = stopwatch.ElapsedMilliseconds;

                            Console.ForegroundColor = ConsoleColor.Green;
                            Console.WriteLine("password: " + line);
                            Console.ForegroundColor = ConsoleColor.White;
                            Console.WriteLine(elapsed + "ms");
                        }

                        if (line == null)
                        {
                            Console.WriteLine("Found nothing");
                        }
                    }
                    Console.Read();
                    break;
            }
        }


        public static void Worker1()
        {
            Console.WriteLine("Thread 1 Initialized");
            string password = _password;
            int debut = _debut;
            int fin = _fin;
            string crack = "";
            char rand;
            int num;
            int lenght;
            int i = 0;
            Random random = new Random();
            //Generation random d'un pseudo mot de passe et verification sur la thread 1

            do
            {
                crack = "";
                lenght = 0;
                i = 0;
                lenght = random.Next(debut, fin);
                while (i != lenght)
                {
                    num = random.Next(0, 26);
                    rand = (char)('a' + num);
                    crack = crack.Insert(0, rand.ToString());
                    i++;
                }
                count++;
            } while (crack != password);
            _crack = crack;
            fini = true;
        }

        public static void Worker2()
        {
            Console.WriteLine("Thread 2 Initialized");
            string password = _password;
            int debut = _debut;
            int fin = _fin;
            string crack = "";
            char rand;
            int num;
            int lenght;
            int i = 0;
            Random random = new Random();
            //Generation random d'un pseudo mot de passe et verification sur la thread 1
            do
            {
                crack = "";
                lenght = 0;
                i = 0;
                lenght = random.Next(debut, fin);
                while (i != lenght)
                {
                    num = random.Next(0, 26);
                    rand = (char)('a' + num);
                    crack = crack.Insert(0, rand.ToString());
                    i++;
                }
                count++;
            } while (crack != password);
            count++;
            _crack = crack;
            fini = true;
        }

        public static void Worker3()
        {
            Console.WriteLine("Thread 3 Initialized");
            string password = _password;
            int debut = _debut;
            int fin = _fin;
            string crack = "";
            char rand;
            int num;
            int lenght;
            int i = 0;
            Random random = new Random();
            //Generation random d'un pseudo mot de passe et verification sur la thread 1
            do
            {
                crack = "";
                lenght = 0;
                i = 0;
                lenght = random.Next(debut, fin);
                while (i != lenght)
                {
                    num = random.Next(0, 26);
                    rand = (char)('a' + num);
                    crack = crack.Insert(0, rand.ToString());
                    i++;
                }
                count++;
            } while (crack != password);
            _crack = crack;
            fini = true;
        }

        public static void Worker4()
        {
            Console.WriteLine("Thread 4 Initialized");
            string password = _password;
            int debut = _debut;
            int fin = _fin;
            string crack = "";
            char rand;
            int num;
            int lenght;
            int i = 0;
            Random random = new Random();
            //Generation random d'un pseudo mot de passe et verification sur la thread 1
            do
            {
                crack = "";
                lenght = 0;
                i = 0;
                lenght = random.Next(debut, fin);
                while (i != lenght)
                {
                    num = random.Next(0, 26);
                    rand = (char)('a' + num);
                    crack = crack.Insert(0, rand.ToString());
                    i++;
                }
                count++;
            } while (crack != password);
            _crack = crack;
            fini = true;
        }
    }
}
