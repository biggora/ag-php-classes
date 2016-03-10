
# Градиентная заливка #
Пример создания изображения с градиентной заливкой.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_dest = './images/test.gif'; 

$prefix = ''; // Приставка к имени файла 
$format = 'gif'; // формат для сохранения изображения

$width = 200; // ширина изображения
$height = 100; // высота изображения
$direction = 'ellipse'; // направление заливки
/*
возможные варианты заливки
'horizontal'
'vertical'
'ellipse'
'ellipse2'
'circle'
'circle2'
'square'
'rectangle'
'diamond'
*/  
$start_color = '#5E0B5F'; // начальный цвет
$end_color = '#fff'; // конечный цвет
$step = 0; //

if($gradient_image = ImagesHelper::gradientfill($width, $height, $direction, $start_color, $end_color, $step))
{
   // сохранение полученного изображения в gif формате 
   ImagesHelper::save($gradient_image, $image_dest, $prefix, $format);   
}

```
![https://lh4.googleusercontent.com/-Z0w7eE6Dd6U/Tj8RpiNuLXI/AAAAAAAALG0/EzyJp_cEKbE/gr1_source.png](https://lh4.googleusercontent.com/-Z0w7eE6Dd6U/Tj8RpiNuLXI/AAAAAAAALG0/EzyJp_cEKbE/gr1_source.png)
![https://lh6.googleusercontent.com/-ejQeM_iG3Rw/Tj8Rp3OLJTI/AAAAAAAALG4/U-UfdkiWSrw/gr2_source.png](https://lh6.googleusercontent.com/-ejQeM_iG3Rw/Tj8Rp3OLJTI/AAAAAAAALG4/U-UfdkiWSrw/gr2_source.png)
![https://lh3.googleusercontent.com/-qtxEg_IUY1c/Tj8Rp-4wYqI/AAAAAAAALG8/rmRQ-rYNI48/gr3_source.png](https://lh3.googleusercontent.com/-qtxEg_IUY1c/Tj8Rp-4wYqI/AAAAAAAALG8/rmRQ-rYNI48/gr3_source.png)

#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>