# Инициирование файла для проги
1. Добавление описания программы 

Для решения данной задачи были использованы 2 массива типа *string. (FirstArray и FinalArray)*

**FirstArray**- объявлен и проинициализирован сразу.
FinalArray был инициализирован с помощью null.

Переменная **n** выступает в роли счетчика элементов, удовлетворяющих условию *coutSymbols <= 3.*

Для выполения отбора и записи в новый массив был использован цикл **foreach.**
При нахождении элемента, удовлетворяющего условию, с помощью свойства *String.Length* , счетчик
верных элементов увеличивается на **1**,
**FinalArray** меняет свой размер с помощью метода *System.Array.Resize(..)*,
в только что добавленный пустой элемент записывается значение найденного и потом из FinalArray выводится значение
в консоль Console.WriteLine(FinalArray[n-1]).

2. Добавление тела программы 

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

# Добавление диаграммы 
3. Добавляем диаграмму 

![что то пошло не так](Algorithm.jpg)



