Reference VS Value types
========================

- Value types
- Reference types 
- Стек
- Куча

Типы в C# можно разделить на типы значений (Value types) и ссылочные типы (Reference types).

### Value types -  значимые типы ###
 
Value types включают большинство встроенных типов:

- Целочисленные типы (byte, sbyte, char, short, ushort, int, uint, long, ulong)
- Типы с плавающей запятой (float, double)
- Тип decimal
- Тип bool

А также специальные типы:

- Перечисления enum
- Структуры (struct)

Пример

    public struct Point {public int X, Y;}

    Point p1 = new Point();
    p1.X = 7;

    Point p2 = p1; //Присваивание приводит к копированию

    Console.WriteLine(p1.X);  //7
    Console.WriteLine(p2.X);  //7

    p1.X = 9; //Изменим p1.X
     Console.WriteLine(p1.X);  //9
    Console.WriteLine(p2.X);  //7

### Reference types - ссылочные типы ###

Reference types включают в себя 
- Тип object
- Тип string
- Классы (class)
- Интерфейсы (interface)
- Делегаты (delegate)

Reference types сложнее Value types из-за наличия двух частей: Объекта и ссылки на этот объект. Содержимым переменной или константы ссылочного типа являеться ссылка на объект, который содержит значение

Пример

    public class Point {public int X, Y;}

    Point p1 = new Point();
    p1.X = 7;

    Point p2 = p1; //Копирует ссылку на p1

    Console.WriteLine(p1.X);  //7
    Console.WriteLine(p2.X);  //7

    p1.X = 9; //Изменим p1.X
     Console.WriteLine(p1.X);  //9
    Console.WriteLine(p2.X);  //9

Присваивание переменной ссылочного типа вызывает копирование ссылки. но не экземпляра объекта. Что позволяет множеству переменных ссылаться на один и тот же объект - с типами значений обычно такое не возможно 

Отличие между Value types и Reference types связано с тем, как они поддерживаются в памяти.
Память в .NET делится на два типа: стек и куча (heap).

Value types данные  хранятся в стеке

Reference types -  данные  хранятся в куче. Куча - это область памяти, в которой размещаются управляемые объекты, и работает сборщик мусора. Сборщик мусора освобождает все ресурсы и объекты, которые уже не нужны.

Стек и куча - это места, где располагаются переменные и константы. Стек и куча имеют существенно отличающуюся семантику времен жизни.

### Стек ###
Стек — представляющий собой список элементов, организованных по принципу LIFO. 

Размер стека составляет 1 МБ для 32 - бит. и 4 МБ для 64 - бит. процессов.

Стек представляет собой блок памяти для хранения локальных переменных и параметров. Стек логически увеличивается при входе в функцию и уменьшается после выхода из нее.

    static int Factorial (int x)
    {
        if(x == 0) return 1;
        return x * Factorial (x-1);
    }

Пример метода является рекурсивным, т.е. он вызывает сам себя. Каждый раз, когда происходит вход в метод, в стеке размещается экземпляр int, а когда метод завершается, экземпляр int освобождается.

### Куча (heap) ###

Куча - это блок памяти, в котором располагаются объекты (экземпляры сылочного типа). Когда создается новый объект, он распределяется в куче с возращением ссылки на этот объект. Во время выполнения программы куча начинает заполняться по мере создания новых объектов. 
В исполняющей среде предусмотрен сборщик мусора, который переодически освобождает объект из кучи. Объект становится пригодным для очистки если отсутствуют ссылки на него.

В куче также хранятся статические поля и константы. В отличие от объектов, распределенных  в куче (которые могут быть обработаны сборщиком мусора), они существуют до тех пор , пока домен не прекратит своего существования.


http://qaru.site/questions/29711/why-is-stack-size-in-c-exactly-1-mb