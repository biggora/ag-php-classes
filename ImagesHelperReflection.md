
# Изображение с отражением #
Пример демонстрирует создание отражения и изображения с отражением.
### Отражение изображения ###
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'ref_'; // Приставка к имени файла отражения 
$format = 'png'; // формат для сохранения изображения

$reflection_height = 25; # %

// Создаем отражение изображения
if($image_reflection  = ImagesHelper::onlyreflection($image_source,$reflection_height)) {
   // сохранение полученного изображения в png формате 
   ImagesHelper::save($image_reflection, $image_source,$prefix,$format);
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh4.googleusercontent.com/-C0bixbDTMwE/Tj-AF4LJByI/AAAAAAAALIQ/lsHlsdLk80Q/ref_source.png](https://lh4.googleusercontent.com/-C0bixbDTMwE/Tj-AF4LJByI/AAAAAAAALIQ/lsHlsdLk80Q/ref_source.png)
### Изображение с отражением ###
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'wref_'; // Приставка к имени файла с отражением 
$format = 'png'; // формат для сохранения изображения

// Создание изображения с отражением 
if($image_with_reflection  = ImagesHelper::reflection($image_source)) {    
    // сохранение полученного изображения в png формате 
    // Примечание: изображение с отражением следует сохранять только в png формате
    ImagesHelper::save($image_with_reflection, $image_source, $prefix, $format);    
}

```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh5.googleusercontent.com/-7n_IJmMgjUI/Tj8RrRBQTHI/AAAAAAAALHQ/Rxc-H7Vpl3c/wref_source.png](https://lh5.googleusercontent.com/-7n_IJmMgjUI/Tj8RrRBQTHI/AAAAAAAALHQ/Rxc-H7Vpl3c/wref_source.png)


---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
