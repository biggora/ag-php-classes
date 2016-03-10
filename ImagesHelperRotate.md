
# Вращение изображения #
#### Вращение изображения Пример 1 ####
Вращение изображения оставляя фон прозрачным.
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'rtdt_'; // Приставка к имени файла 
$format = 'png'; // формат для сохранения изображения

$degrees = 55; // угол поворота в градусах

// Вращаем изображение оставляя фон прозрачным
if($rotated_image = ImagesHelper::rotate($image_source,$degrees))
{
   // сохранение полученного изображения в png формате 
   ImagesHelper::save($rotated_image, $image_source,$prefix,$format);    
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh5.googleusercontent.com/-9LR_Y60QrgE/Tj9_MumziDI/AAAAAAAALH8/doC4vntX4VI/rtdf_source.png](https://lh5.googleusercontent.com/-9LR_Y60QrgE/Tj9_MumziDI/AAAAAAAALH8/doC4vntX4VI/rtdf_source.png)
#### Вращение изображения Пример 2 ####
Вращение изображения делая заливку фона определенным цветом
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'rtdс_'; // Приставка к имени файла
$format = 'png'; // формат для сохранения изображения

$degrees = 75; // угол поворота в градусах
$bg_color = '#7E58BF'; // цвет фоновой заливки
$transparent = false;  // прозрачность

// Вращаем изображение делая заливку фона определенным цветом 
if($rotated_image = ImagesHelper::rotate($image_source, $degrees, $bg_color, $transparent))
{
   // сохранение полученного изображения в png формате 
   ImagesHelper::save($rotated_image, $image_source, $prefix, $format);    
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh3.googleusercontent.com/-yD9Fo5QIjYk/Tj8Rq2EszYI/AAAAAAAALHM/jSs-TihCamA/rtdt_source.png](https://lh3.googleusercontent.com/-yD9Fo5QIjYk/Tj8Rq2EszYI/AAAAAAAALHM/jSs-TihCamA/rtdt_source.png)

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
