
# Наложение изображения #
Пример быстрого наложения одного изображения на другое.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$prefix = 'ovr_'; // Приставка к имени файла 
$format = 'gif'; // формат для сохранения изображения
$overlay_img = './images/wtm.gif'; // накладываемое изображение
$alpha_level   = 30; // прозрачность накладываемого изображения
$position = 'center'; // позиция
/*
 *  доступные позиции
 * 'top-right','right-top',1
 * 'top-left','left-top',2
 * 'bottom-right','right-bottom',3
 * 'bottom-left','left-bottom',4
 * 'center',5
 * 'top',6
 * 'bottom',7
 * 'left',8
 * 'right',9
 */
if($overlayed_image = ImagesHelper::overlay($image_source, $overlay_img,$position,$alpha_level)) {
   // сохранение полученного изображения в gif формате
   ImagesHelper::save($overlayed_image, $image_source, $prefix, $format); 
   // или вывести изображение в броузер
   ImagesHelper::show($overlayed_image);   
}
```
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>