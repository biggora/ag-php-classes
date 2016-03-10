
# Информация об изображении #
Примеры получения основной информации об изображении.
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 
  
// получение размера изображения  
$width      = ImagesHelper::width($image_source); 
$height     = ImagesHelper::height($image_source);  

// Получение типа изображения 
$mime       = ImagesHelper::mime($image_source);
```


---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
