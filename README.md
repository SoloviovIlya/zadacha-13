//Напишите программу, которая выводит третью цифру заданного числа или сообщает, что третьей цифры нет.
//645 -> 5
//78 -> третьей цифры нет
//32679 -> 6

Console.WriteLine("Введите число: ");

int a = Convert.ToInt32(Console.ReadLine());

int i = 0;

int b = a;

int c = 0;

while (a%10 != 0)

{

    a = a / 10;
    
    i = i+1; 
}

if (i < 3)

{
    Console.WriteLine("Третьей цифры нет");
}

else

{
    while (i != 3)
    
    {
        c = b / 10;
        
        b = c;
        
        i = i-1;
    }
    
    Console.WriteLine($"Третья цифра - {c%10}");
    
}
