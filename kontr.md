# Инициирование файла для проги

1. Добавление теда программы 

namespace ConsoleApp8

{
    class Program
    
    {
        static void Main(string[] args)
        {
            // Инициализация массива строк
            string[] FirstArray = { "H3i", "Hello", "Good morning",
                            "521", "Sa-y", "Mexico", "Switch",
                            "5-1", "Sa'1y", ">/]", "Switch" };

            string[] FinalArray = null;

            int n = 0;

            //Отбор нужных элементов, запись в массив и вывод на экран
            foreach(string s in FirstArray)
            {
                if(s.Length <= 3)
                {
                    n += 1;
                    System.Array.Resize(ref FinalArray, n);

                    FinalArray[n-1] = s;

                    Console.WriteLine(FinalArray[n-1]);
                }
            }
        }
    }
}

# добавление диаграммы 
Добавляем диаграмму 
![что то пошло не так](Algorithm.jpg)


