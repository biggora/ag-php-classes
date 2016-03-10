
# Водяные знаки #
#### Водяные знаки Пример 1 ####
Пример создания водяного знака с помощью изображения.
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
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh5.googleusercontent.com/-jJITTU-GXFo/Tj--f-OCh0I/AAAAAAAALJA/yFOdIa7GnU4/wtmi3_source.gif](https://lh5.googleusercontent.com/-jJITTU-GXFo/Tj--f-OCh0I/AAAAAAAALJA/yFOdIa7GnU4/wtmi3_source.gif)
#### Водяные знаки Пример 2 ####
Пример создания водяного знака с помощью текста.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/source.jpg'; 

$prefix = 'wtmt_'; // Приставка к имени файла с отражением 
$format = 'png'; // формат для сохранения изображения

$text = "OVERLEY TEXT";
$path_to_font = './fonts/Yahoo.ttf';
$color = '#ccc'; //#5E0B5F';

$alpha_level = 50; // уровень прозрачности
$position    = 'bottom-right';
$angle       = 0; // угол поворота текста в градусах

if($watermarked_image = ImagesHelper::overlaytext( $image_source, $text, $path_to_font, $color, 
                                                   $position, $alpha_level, $angle)) {
   // сохранение полученного изображения в png формате 
  ImagesHelper::save($watermarked_image, $image_source, $prefix, $format);

}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh3.googleusercontent.com/-3nc2krGWAa4/Tj8RrjaFt8I/AAAAAAAALHU/joWpEO4-UmM/wtmt_source.png](https://lh3.googleusercontent.com/-3nc2krGWAa4/Tj8RrjaFt8I/AAAAAAAALHU/joWpEO4-UmM/wtmt_source.png)

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>