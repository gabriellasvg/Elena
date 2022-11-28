// Задача 43: Напишите программу, которая найдёт точку пересечения двух прямых, 
// заданных уравнениями y = k1 * x + b1, y = k2 * x + b2; значения b1, k1, b2 и k2 
// задаются пользователем.
// b1 = 2, k1 = 5, b2 = 4, k2 = 9 -> (-0,5; -0,5)

Консоль. Write("Введите k1:");
vark1=Конвертировать. ToDouble(Консоль. ЧитатьЛинию());
Консоль. Write("Введите b1:");
varb1=Преобразовать. ToDouble(Консоль. ЧитатьЛинию());
Консоль. Write("Введите k2:");
vark2=Конвертировать. ToDouble(Консоль. ЧитатьЛинию());
Консоль. Write("Введите b2:");
varb2=Конвертировать. ToDouble(Консоль. ЧитатьЛинию());
 
 
varx=-(b1-b2)/(k1-k2);
var y = k1 * x + b1;
 
x=Математика. Круглый(x,3);
y=Математика. Круглый(y,3);
 
Консоль. WriteLine($"Пересечение в точке: ({x};{ y}) ");

//Пользователь вводит с клавиатуры M чисел. Посчитайте, сколько чисел больше 0 ввёл пользователь.

Console.Write("Введите элементы(через пробел): ");
int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);
int count = 0;
 
for (int i = 0; i < arr.Length; i++)
{
    if (arr[i] > 0)
    {
        count++;
    }
}
 
Console.WriteLine($"Кол-во элементов > 0: {count}");
