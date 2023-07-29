
# <span>__Решение домашних заданий к семинару 2. Исключения и их обработка.__</span>

## **Задача 1.**

Реализуйте метод, который запрашивает у пользователя ввод дробного числа (типа float), и возвращает введенное значение. Ввод текста вместо числа не должно приводить к падению приложения, вместо этого, необходимо повторно запросить у пользователя ввод данных.

[Решение]()

## **Задача 2.**

Если необходимо, исправьте данный код ([задание 2](https://docs.google.com/document/d/17EaA1lDxzD5YigQ5OAal60fOFKVoCbEJqooB9XfhT7w/edit))

**Решение:**

1. Код не скомпилируется так как не задан массив intArray[8]:
       
        double catchedRes1 = intArray[8] / d;

## **Задача 3.**

Дан следующий код, исправьте его там, где требуется ([задание 3](https://docs.google.com/document/d/17EaA1lDxzD5YigQ5OAal60fOFKVoCbEJqooB9XfhT7w/edit))

**Решение:**

1. Лишнее throws Exception при объявлении метода main так как все ошибки обрабатываются в дальнейшем:

       public static void main(String[] args) throws Exception 

2. Лишняя обработка так как нулевых значений в коде не наблюдается, все ошибки ловит первый catch (Throwable ex):

       catch (NullPointerException ex) {
            System.out.println("Указатель не может указывать на null!");
       }

3. Лишнее throws FileNotFoundException при объявлении метода так как нет работы с файлами в коде:

       public static void printSum(Integer a, Integer b) throws FileNotFoundException {
            System.out.println(a + b);
       }

## **Задача 4.**

Разработайте программу, которая выбросит Exception, когда пользователь вводит пустую строку. Пользователю должно показаться сообщение, что пустые строки вводить нельзя.

[Решение]()



