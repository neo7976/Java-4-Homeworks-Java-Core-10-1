# Java-4-Homeworks-Java-Core-10-1
Задача "Понимание JVM"

[Этапы в области памяти](https://github.com/neo7976/Java-4-Homeworks-Java-Core-10-1/blob/main/file/%D0%94%D0%97%20-%20%D0%B2%D1%81%D0%B5%20%D1%8D%D1%82%D0%B0%D0%BF%D1%8B.pdf)

- Наш исходный код 
![](img/0001.jpg)
 
- Происходит добавление JvmComprehension в Metaspace
![](img/0002.jpg)
   
- Создается `main()` в стеке
![](img/0003.jpg)
 
- Создается переменная `i` в main()
![](img/0004.jpg) 

- Создаем `Object` в heap (куче)
![](img/0005.jpg) 

- Создается переменная `o` в main() с сылкой на `Object`
![](img/0006.jpg) 

- Создаем `Integer` в heap (куче)
![](img/0007.jpg) 

- Создается переменная `ii` в main() с сылкой на `Integer`
![](img/0008.jpg) 

- Создается `printAll()` в стеке
![](img/0009.jpg)

- Создается переменная `o`, `ii` и `i` в printAll() с ссылкой на `Object` `Integer` соответственно
![](img/0010.jpg) 

- Создается переменная `userlessVar` в printAll() с ссылкой на `Integer`
![](img/0011.jpg) 

- Передаем новый фрейм в стек, куда передаем ссылку на результат `о`, `i` и `ii`
![](img/0012.jpg) 

- Передаем новый фрейм в стек и выводим сообщение об окончании выполняемой программы
![](img/0013.jpg) 


