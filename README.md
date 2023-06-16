
<h2 align="center">ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ПРОФЕССИОНАЛЬНОГО ОБРАЗОВАНИЯ <br> «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ» <br> КАФЕДРА ИНФОРМАТИКИ </h2>
<p align="center">Лабораторная работа №12 <br>
по курсу «Web-технологии, языки и средства создания web-приложений» 

<p align="center"><b>"PHP"</b><p>
<p align="right"><b>Выполнила: </b> студентка 231 группы Витковская Полина</p>
<p  align="right"><b>Принял: </b> Соболев Е. И., старший преподователь</p>
<br>
<br>
<br>
<p align="center">Южно-Сахалинск <br> СахГУ <br> 2023</p>
<h2> Введение </h2>
<p>Лабораторные работы по дисциплине «Web-технологии, языки и средства создания web-приложений» предназначены для освоения полученных теоретических знаний на практике. Цель работы - выполнить задачи, написав решение на PHP.  <br>

</p>
<h2>Решение задач</h2>

1. 
```php
$array = range(1,100);
echo array_sum($array);
```
2. 
```php
$array = array("a","b","c","d","e");
$array = array_map("strtoupper",$array); 
print_r($array);

```
3. 
```php
$array = range(1, 50);
echo count($array);
```
4. 
```php
$array = range(50, 75);
echo $array[count($array) - 1];
```
5. 
```php
function f($array)
{
	for($i = 0; $i < count($array); $i++)
    {
    	if($array[$i] == 3)
        {
        	return true;
        }
    }
    return false;
}
```
6. 
```php
$array = range(1,5);
echo array_sum($array);
```
7. 
```php
$array = range(1,5);
$res = 1;
for($i = 0; $i < count($array); $i++)
{
	$res *= $array[$i];
}
echo $res;
```
8. 
```php
$array = range(1,100);
echo array_sum($array)/count($array);
```
9. 
```php
$array = range(1,100);
```
10. 
```php
$array = range('a','z');
```
11. 
```php
$array = range(1,9);
echo implode($array, "-");
```
12. 
```php
$array = range(1,100);
```
13. 
```php
$array = range(1,10);
echo array_product($array);
```
14. 
```php
$a = array(1,2,3);
$b = array('a','b','c');
print_r(array_merge($a, $b));
```
15. 
```php
$array = range(1,5);
$result = array_slice($array, 1,3);
print_r($result);
```
16. 
```php
$array = range(1,5);
array_splice($array, 1, 2);
print_r($array);
```
17. 
```php
$array = range(1,5);
$array2 = array_splice($array, 1, 3);
print_r($array2);
```
18. 
```php
$array = range(1,5);
array_splice($array, 3, 0,array('a','b','c'));
print_r($array);
```
19. 
```php
$array = range(1,5);
array_splice($array, 1, 0,array('a','b'));
array_splice($array, 6, 0, 'c');
array_splice($array, 8, 0, 'e');
print_r($array);
```
20. 
```php
$array = array('a'=>1, 'b'=>2, 'c'=>3);
$keys = array_keys($array);
$values = array_values($array);
print_r($keys);
echo "<br>";
print_r($values);
```
21. 
```php
$keys = array('a','b','c');
$values = array(1,2,3);
$array = array_combine($keys, $values);
print_r($array);
```
22. 
```php
$array = array('a'=>1, 'b'=>2, 'c'=>3);
$array = array_flip($array);
print_r($array);
```
23. 
```php
$array = range(1,5);
$array = array_reverse($array);
print_r($array);
```
24. 
```php
$array = array('a','-','b','-','c','-','d');
echo array_search('-',$array);
```
25. 
```php
$array = array('a','-','b','-','c','-','d');
array_splice($array, array_search('-', $array), 1);
print_r($array);
```
26. 
```php
$array = array('a','-','b','-','c','-','d');
$array[0] = '!';
$array[3] = '!!';
print_r($array);
```
27. 
```php
$array = array('3'=>'a', '1'=>'c', '2'=>'e', '4'=> 'b');
$new=arsort($array);
print_r($new);
$new=asort($array);
print_r($new);
$new=array_multisort($array);
print_r($new);
$new=sort($array);
print_r($new);

```
28. 
```php
$array = array('a'=>1,'b'=>2,'c'=>3);
echo array_rand($array);
```
29. 
```php
$array = array('a'=>1,'b'=>2,'c'=>3);
echo $array[array_rand($array)];
```
30. 
```php
$arr = range(1,5);
shuffle($array);
print_r($array);
```
31. 
```php
$arr = range(1, 25);
shuffle($arr);
print_r($arr);
```
32. 
```php
$arr = range('a','z');
shuffle($arr);
print_r($arr);
```
33. 
```php
$arr = range('a','z');
shuffle($arr);
$string = '';
for($i = 0; $i < 6; $i++)
	$string.= $arr[$i];
echo $string;
```
34. 
```php
$arr = array('a','b','c','b','a');
print_r(array_unique($arr));

```
35. 
```php
$arr = range(1,5);
echo array_shift($arr);
echo "<br>";
echo array_pop($arr);
```
36. 
```php
$arr = range(1,5);
array_unshift($arr, 0);
array_push($arr, 6);
print_r($arr);
```
37. 
```php
$arr = range(1,8);
for($i = 0; $i < 4; $i++)
{
	echo array_shift($arr);
    echo array_pop($arr);
}
```
38. 
```php
$arr = array('a','b','c');
for($i = 0; $i < 3; $i++)
	array_push($arr, '-');
print_r($arr);
```
39. 
```php
$arr = array();
for($i = 0; $i < 10; $i++)
	array_push($arr, 'x');
print_r($arr);
```
40. 
```php
$arr = range(1,20);
print_r(array_chunk($arr,4));
```

<h2>Вывод</h2>
<p>В ходе лабораторной работы были изучены элементы языка PHP. Были рассмотрены методы и функции массивов, выполнены практические задания.</p>    
