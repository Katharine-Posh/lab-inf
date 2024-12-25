# Лабораторная работа 


## 1. Задание

1. Скопируйте к себе файл data.txt из данного репозитория. Выполните команду:
   
    ```
    grep 'Error' data.txt
    ```

    В результате должны вывестить все строки, в которых содержится слово 'Error':
  
    ```
    2024-12-01 Error: File not found
    2024-12-04 Error: Permission denied
    ```

2.  Далее выполните команду:
   
     ``` 
     grep -n 'Warning' data.txt
     ```

    Флаг `-n` показывает на номер строки, в которой будет содержаться 'Warning'. Ожидаемый вывод:
  
    ```
    2:2024-12-02 Warning: Disk space low
    6:2024-12-06 Warning: High memory usage
    ```

4. Как вывести число строк, содержащих какие либо данные?
   
   ```
   grep 'Error|Warning' data.txt | wc -l
   ```
   
   `wc` - команда для подсчёта строк, слов и байт. В данном случае мы считаем строки. С помощью | мы перенаправили вывод предыдущей команды в следующую, поэтому ожидаемый результат:

   ```
   4
   ```
   

## Задание для самостоятельного выполнения
 
Теперь, работая над файлом text.txt из этого же репозитория, нужно выполнить 3 задания:
1. Выделяя цветом, найти строки, начинающиеся с буквы А
2. Найти строчку с вопросительным предложением. Вывести искомую строчку +2 до и после неё
3. Найти строки, содержащие ';', но не содержащие какое-либо сочетание букв, например 'vel', и сохранить результат в другой текстовый файл


## Ресурсы

1. [Команда grep в Linux](https://selectel.ru/blog/tutorials/grep-command-in-linux/)
2. [Применение команды grep](https://zomro.com/rus/blog/faq/509-grep-command-in-linux)
3. [grep Command in Linux and Unix](https://builtin.com/articles/grep-command#:~:text=The%20grep%20command%20is%20used,or%20output%20from%20other%20commands.)