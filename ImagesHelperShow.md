
# Вывод изображения в броузер #
В Данном примере показано как выполнить вывод изображения в броузер, допускается вывод в различных графических форматах.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

// Создать изображение из файла
$image = ImagesHelper::create($image_source);

// Вывести изображение в броузер
ImagesHelper::show($image);

/*
  Вывод изображения в броузер в определенном формате
  ImagesHelper::show($image,'png');
*/

```
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>