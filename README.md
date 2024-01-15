1. Напишите сценарий, который принимает целое число в качестве аргумента и возвращает «Четное» 
для четных чисел или «Нечетное» для нечетных чисел.

2. Создайте функцию, которая проверяет, делится ли число n на два числа x И y. Все входные 
данные являются положительными, ненулевыми числами.

Пример:
1) n =   3, x = 1, y = 3 =>  true because   3 is divisible by 1 and 3
2) n =  12, x = 2, y = 6 =>  true because  12 is divisible by 2 and 6
3) n = 100, x = 5, y = 3 => false because 100 is not divisible by 3
4) n =  12, x = 7, y = 5 => false because  12 is neither divisible by 7 nor 5



ЗАДАЧА1:
number=$1

if [ $((number % 2)) -eq 0 ]; then
  echo "Четное"
else
  echo "Нечетное"
fi


ЗАДАЧА2:
n=$1
x=$2
y=$3

if [ $((n % x)) -eq 0 ] && [ $((n % y)) -eq 0 ]; then
  echo "true"
else
  echo "false"
fi


ПОЯСНЕНИЕ:
[] - такие скобки для условных выражение, где 0 - тру, 1 - фолз
(()) - такие скобки для арифмитических выраж
-eq - "equal", логическое равно
% - остаток от деления 
