
# Вывод изображения в броузер #
В Данном примере показано как выполнить вывод изображения в броузер, допускается вывод в различных графических форматах.
```php
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


---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
