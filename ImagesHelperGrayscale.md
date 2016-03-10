
# Из цветного изображения в черно-белое или негатив #
#### Черно-белое изображение ####
Пример преобразования цветного изображения в черно-белое.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'bw_'; // Приставка к имени файла 
$format = 'gif'; // формат для сохранения изображения

// конвертируем в черно-белое
if($grayscale_image = ImagesHelper::grayscale($image_source)) {
   // сохранение полученного изображения в gif формате 
   ImagesHelper::save($grayscale_image, $image_source,$prefix, $format);
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh4.googleusercontent.com/-31LrzcmE__Q/Tj8RppAKYeI/AAAAAAAALGw/s5-9jASpqSo/bw_source.gif](https://lh4.googleusercontent.com/-31LrzcmE__Q/Tj8RppAKYeI/AAAAAAAALGw/s5-9jASpqSo/bw_source.gif)
#### Негатив изображения ####
Пример преобразования изображения в негатив.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'ng_'; // Приставка к имени файла 
$format = 'png'; // формат для сохранения изображения

// конвертируем в негатив
if($negative_image  = ImagesHelper::negative($image_source)) {
   // сохранение полученного изображения в png формате 
   ImagesHelper::save($negative_image, $image_source, $prefix, $format);
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh6.googleusercontent.com/-hDxmBuBBPvM/Tj8RqRyRfTI/AAAAAAAALHE/gTCKKK3Ok-A/ng_source.png](https://lh6.googleusercontent.com/-hDxmBuBBPvM/Tj8RqRyRfTI/AAAAAAAALHE/gTCKKK3Ok-A/ng_source.png)
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>