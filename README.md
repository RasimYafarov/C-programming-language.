# C++ для начинающих 
 C++ (читается си-плюс-плюс) — компилируемый, статически типизированный язык программирования общего назначения. 
 
 Поддерживает такие парадигмы программирования, как процедурное программирование, объектно-ориентированное программирование, обобщённое программирование. Язык имеет богатую стандартную библиотеку, которая включает в себя распространённые контейнеры и алгоритмы, ввод-вывод, регулярные выражения, поддержку многопоточности и другие возможности. C++ сочетает свойства как высокоуровневых, так и низкоуровневых языков. В сравнении с его предшественником — языком C — наибольшее внимание уделено поддержке объектно-ориентированного и обобщённого программирования]. 
 
 C++ широко используется для разработки программного обеспечения, являясь одним из самых популярных языков программирования. Область его применения включает создание операционных систем, разнообразных прикладных программ, драйверов устройств, приложений для встраиваемых систем, высокопроизводительных серверов, а также компьютерных игр. Существует множество реализаций языка C++, как бесплатных, так и коммерческих и для различных платформ. Например, на платформе x86 это GCC, Visual C++, Intel C++ Compiler, Embarcadero (Borland) C++ Builder и другие. C++ оказал огромное влияние на другие языки программирования, в первую очередь на Java и C#. 
 
 Синтаксис C++ унаследован от языка C. Изначально одним из принципов разработки было сохранение совместимости с C. Тем не менее C++ не является в строгом смысле надмножеством C; множество программ, которые могут одинаково успешно транслироваться как компиляторами C, так и компиляторами C++, довольно велико, но не включает все возможные программы на C. 
 
Основные типы данных в C++

int — целочисленный тип данных.
float — тип данных с плавающей запятой.
double — тип данных с плавающей запятой двойной точности.
char — символьный тип данных.
bool — логический тип данных.

Объявление переменной

Объявление переменной в C++ происходит таким образом: сначала указывается тип данных для этой переменной а затем название этой переменной.

Пример

int a; // объявление переменной a целого типа. 

float b; // объявление переменной b типа данных с плавающей запятой. 

double c = 14.2; // инициализация переменной типа double. 

char d = 's'; // инициализация переменной типа char. 

bool k = true; // инициализация логической переменной k.

Цикл for

Если мы знаем точное количество действий (итераций) цикла, то можем использовать цикл for. Синтаксис его выглядит примерно так:

for (действие до начала цикла;

     условие продолжения цикла;
     
     действия в конце каждой итерации цикла) {
     
         инструкция цикла;
         
         инструкция цикла 2;
         
         инструкция цикла N;
}

Цикл while

Когда мы не знаем, сколько итераций должен произвести цикл, нам понадобится цикл while или do...while. Синтаксис цикла while в C++ выглядит следующим образом.

while (Условие) {

    Тело цикла;
    
}

Пример обычного калькулятора:

#include <iostream> 
 
using namespace std;

int main() 
 
{ 
    setlocale(0, ""); 
 
    /*7*/ int a, b; // объявление двух переменных a и b целого типа данных. 
 
    cout << "Введите первое число: "; 
 
    cin >> a; // пользователь присваивает переменной a какое-либо значение. 
 
    cout << "Введите второе число: "; 
 
    cin >> b; 
 
    /*12*/  int c = a + b; // новой переменной c присваиваем значение суммы введенных пользователем данных. 
 
    cout << "Сумма чисел = " << c << endl; // вывод ответа.
 
    return 0; 
 
}

Конструкция if:

Конструкция if проверяет истинность условия, и если оно истинно, выполняет блок инструкций. Этот оператор имеет следующую сокращенную форму:

if (условие)

{

    инструкции;
    
}

Конструкция switch:

Другую форму организации ветвления программ представляет конструкция switch...case. Она имеет следующую форму:

switch(выражение)
{

    case константа_1: инструкции_1;
    
    case константа_2: инструкции_2;
     
    default: инструкции;
    
}

