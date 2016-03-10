
# Затемнение изображения #
Пример показывает как затемнять и накладывать цвет на изображение.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'fad_'; // Приставка к имени файла с отражением 
$format = 'png'; // формат для сохранения изображения

$alpha_start = 120;
$alpha_end = 0;
$bg_color = "#000"; // накладываемый цвет (черный)

// Накладываем цвет на изображение
if($faded_image = ImagesHelper::fade($image_source,$alpha_start,$alpha_end,$bg_color)) {
   // сохранение полученного изображения в png формате 
   ImagesHelper::save($faded_image, $image_source, $prefix, $format);  
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh6.googleusercontent.com/-3j227rfk3As/Tj8RpTuBFUI/AAAAAAAALGs/uFtv_-L9csw/fad2_source.png](https://lh6.googleusercontent.com/-3j227rfk3As/Tj8RpTuBFUI/AAAAAAAALGs/uFtv_-L9csw/fad2_source.png)
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>