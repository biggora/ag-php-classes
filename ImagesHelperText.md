
# Текст как изображение #
Примеры как создать текст в виде изображения.
#### Текст как изображение Пример 1 ####
Создание изображения с текстом, с произвольным выбором цвета текста и фона.
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/text.jpg'; 

$text = "ImagesHelper"; // текст
$path_to_font = './fonts/BeAggressive.ttf'; // путь к файлу с фонтом
$text_color = '#ffffff'; // цвет текста
/* если значение переменной $text_color = false текст будет прозрачным */
$bg_color = '#5E0B5F'; // цвет фона 
/* если значение переменной $bg_color = false фон будет прозрачным */
$font_size = 30; // размер шрифта
$format = 'png'; // формат для сохранения изображения

// Создаем текст как изображение
if($image_text  = ImagesHelper::text($text,$font_size,$path_to_font,$text_color,$bg_color)) {
  // вывести изображение в броузер как png
  ImagesHelper::show($image_text,$format,100);
}
```
![https://lh5.googleusercontent.com/-ia6pTwWtLq4/Tj8S-t23wQI/AAAAAAAALHc/FwHWafxoR3w/s1024/txt3_source.png](https://lh5.googleusercontent.com/-ia6pTwWtLq4/Tj8S-t23wQI/AAAAAAAALHc/FwHWafxoR3w/s1024/txt3_source.png)
#### Текст как изображение Пример 2 ####
Создание изображения с текстом на прозрачном фоне, в место цвета текста использовано другое изображение.
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/text_2.png'; 

$path_to_font = './fonts/Bleeding_Cowboys.ttf'; // путь к файлу с фонтом
$text = "ImagesHelper"; // текст
$image_bg = './images/rainbow.jpg'; // изображение для заливки надписи
$bg_color = false; // цвет фона (прозрачный)
$format = 'png'; // формат для сохранения изображения

if($image_text = ImagesHelper::textto( $image_bg, $text, $font_size, $path_to_font, $bg_color)) {
   // вывести изображение в броузер как gif
   ImagesHelper::save($image_text, $image_source, 'txto2_', 'gif');
}
```
![https://lh5.googleusercontent.com/-I8BOUkU6lL8/Tj8Rq6gWq2I/AAAAAAAALHI/ctZM4xi9v7M/txto2_source.gif](https://lh5.googleusercontent.com/-I8BOUkU6lL8/Tj8Rq6gWq2I/AAAAAAAALHI/ctZM4xi9v7M/txto2_source.gif)

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
