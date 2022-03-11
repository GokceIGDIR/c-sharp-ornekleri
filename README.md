# c-sharp-ornekleri
// ikinci dereceden denklemin kökleri bulmaya yardımcı
static void Main(string[] args)
        {
            double a, b, c, delta, x1, x2;
            Console.WriteLine("ax2 + bx + c = 0  denklemi için ;");
            Console.Write("a katsayısını girin:");
            a = Convert.ToDouble(Console.ReadLine());
            Console.Write("b katsayını girin:");
            b = Convert.ToDouble(Console.ReadLine());
            Console.Write("c katsayısını girin:");
            c = Convert.ToDouble(Console.ReadLine());
            delta = b * b - 4 * a * c;

            if (delta > 0)
            {
                x1 = (-b + Math.Sqrt(delta)) / (2 * a);
                x2 = (-b - Math.Sqrt(delta)) / (2 * a);
                Console.WriteLine("1.kök = {0}", x1);
                Console.WriteLine("2.kök = {0}", x2);
            }
            else if (delta == 0)
            {
                x1 = -b / (2 * a);
                Console.WriteLine("Tek kök = {0}", x1);
            }
            else
            {
                Console.WriteLine("Reel kök yoktur!");
            }
            Console.ReadKey();
        }
        

