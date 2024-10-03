////задание 1
//class Program
//{
//    static double Res(double x)
//    {
//        if (x % 2 != 0)
//        {
//            Console.WriteLine(x = 0);
//            return x;
//        }
//        else
//        {
//            Console.WriteLine(x = x - 2);
//            return x;
//        }

//    }
//    static void Main(string[] args)
//    {
//        double x = Convert.ToDouble(Console.ReadLine());

//        Console.WriteLine(Res(x));
//    }
//}


////задание 2

//class Prog
//{
//    static double Res(double x)
//    {
//        if (x % 5 != 0)
//        {
//            Console.WriteLine(x = x + 1);
//            return x;
//        }
//        else
//        {
//            Console.WriteLine(x = x / 5);
//            return x;
//        }

//    }
//    static void Main(string[] args)
//    {
//        double x = Convert.ToDouble(Console.ReadLine());

//        Console.WriteLine(Res(x));
//    }
//}


////задание 3

//class Pr
//{
//    static int Num(int x)
//    {
//        if (x >= 10 && x <= 99)
//        {
//            int numOne = x / 10;
//            int numTwo = x % 10;
//            return numTwo * 10 + numOne;
//        }
//        else
//        {
//            return x;
//        }
//    }

//    static void Main(string[] args)
//    {
//        Console.WriteLine("Введите число: ");
//        int num = Convert.ToInt32(Console.ReadLine());
//        int result = Num(num);
//        Console.WriteLine(result);
//    }
//}

////задание 4

//class Pr0gram
//{
//    static int Num(int x)
//    {
//        if (x >= 99 && x <= 999)
//        {
//            int numOne = x / 100;
//            int numTwo = (x % 100) / 10;
//            int numThree = x % 10;
//            return numThree * 100 + numTwo * 10 + numOne;
//        }
//        else
//        {
//            return x;
//        }
//    }

//    static void Main(string[] args)
//    {
//        Console.WriteLine("Введите число: ");
//        int num = Convert.ToInt32(Console.ReadLine());
//        int result = Num(num);
//        Console.WriteLine(result);
//    }
//}

//задание 5

public class Program
{
    public static double Form(double a, double b)
    {
        return Math.Sqrt(a * a + b * b);
    }

    public static void Main(string[] args)
    {
        Console.WriteLine("Введите длину стороны AB: ");
        double AB = double.Parse(Console.ReadLine());

        Console.WriteLine("Введите длину стороны AC: ");
        double AC = double.Parse(Console.ReadLine());

        Console.WriteLine("Введите длину стороны DC: ");
        double DC = double.Parse(Console.ReadLine());

        double BC = Form(AB, AC);
        double AD = Form(DC, BC);
        double perimeter = AB + BC + DC + AD;

        Console.WriteLine("Периметр фигуры ABCD:" + perimeter);
    }
}
