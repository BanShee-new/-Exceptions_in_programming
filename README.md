# Exceptions

## HomeWork1. Обработка ошибок в программировании

1. Реализуйте 3 метода, чтобы в каждом из них получить разные исключения
2. Посмотрите на код, и подумайте сколько разных типов исключений вы тут сможете получить?
```markdown
public static int sum2d(String[][] arr) {
  int sum = 0;
  for (int i = 0; i < arr.length; i++) {
    for (int j = 0; j < 5; j++) {
      int val = Integer.parseInt(arr[i][j]);
      sum += val;
    }
  }
return sum;
}
```
3. "*" Реализуйте метод, принимающий в качестве аргументов два целочисленных массива, и возвращающий новый массив, каждый элемент которого равен частному элементов 
двух входящих массивов в той же ячейке. Если длины массивов не равны, необходимо как-то оповестить пользователя. 
Важно: При выполнении метода единственное исключение, которое пользователь может увидеть - RuntimeException, т.е. ваше.


## HomeWork2. Исключения и их обработка

1. Реализуйте метод, который запрашивает у пользователя ввод дробного числа (типа float),
и возвращает введенное значение. 
Ввод текста вместо числа не должно приводить к падению приложения, 
вместо этого, необходимо повторно запросить у пользователя ввод данных.


2. Если необходимо, исправьте данный код

Код 2.1:
```markdown
>try {<p>
   int d = 0<p>
   double catchedRes1 = intArray[8] / d;<p>
   System.out.println("catchedRes1 = " + catchedRes1);<p>
} catch (ArithmeticException e) {<p>
   System.out.println("Catching exception: " + e);<p>
}
```
Код 2.2:
```markdown
>public static void main(String[] args) throws Exception {<p>
   try {<p>
       int a = 90;<p>
       int b = 3;<p>
       System.out.println(a / b);<p>
       printSum(23, 234);<p>
       int[] abc = { 1, 2 };<p>
       abc[3] = 9;<p>
   } catch (Throwable ex) {<p>
       System.out.println("Что-то пошло не так...");<p>
   } catch (NullPointerException ex) {<p>
       System.out.println("Указатель не может указывать на null!");<p>
   } catch (IndexOutOfBoundsException ex) {<p>
       System.out.println("Массив выходит за пределы своего размера!");<p>
   }<p>
}<p>
public static void printSum(Integer a, Integer b) throws FileNotFoundException {<p>
   System.out.println(a + b);<p>
}
```
3. Разработайте программу, которая выбросит Exception, когда пользователь вводит пустую строку. Пользователю должно показаться сообщение, что пустые строки вводить нельзя.


