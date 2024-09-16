using System;

class Program
{
    static void Main()
    {
        int n = 6;  // حجم القلب

        // الجزء العلوي من القلب
        for (int i = n / 2; i <= n; i += 2)
        {
            // المسافات الفارغة على اليسار
            for (int j = 1; j < n - i; j += 2)
            {
                Console.Write(" ");
            }

            // النجوم في النصف الأيسر
            for (int j = 1; j <= i; j++)
            {
                Console.Write("*");
            }

            // المسافات الفارغة بين نصفين القلب
            for (int j = 1; j <= n - i; j++)
            {
                Console.Write(" ");
            }

            // النجوم في النصف الأيمن
            for (int j = 1; j <= i; j++)
            {
                Console.Write("*");
            }

            // الانتقال إلى السطر التالي
            Console.WriteLine();
        }

        // الجزء السفلي من القلب
        for (int i = n; i >= 1; i--)
        {
            // المسافات الفارغة على اليسار
            for (int j = i; j < n; j++)
            {
                Console.Write(" ");
            }

            // النجوم في الجزء السفلي
            for (int j = 1; j <= (i * 2) - 1; j++)
            {
                Console.Write("*");
            }

            // الانتقال إلى السطر التالي
            Console.WriteLine();
        }
    }
}
