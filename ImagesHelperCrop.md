
# Обрезка, сложное масштабирование изображения #
Иногда требуется из прямоугольного изображения сделать квадратное с сохранением всех пропорций. С помощью ImagesHelper сделать это легко, как показано в описанном ниже примере

#### Сложное масштабирование ####
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$ratio = 70; // соотношение в % от основного изображения

if($quadrate_image  = ImagesHelper::quadrate($image_source,$ratio)) { 
   // сохранение полученного изображения в gif формате   
   ImagesHelper::save($quadrate_image, $image_source,'qua_','gif'); 
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh3.googleusercontent.com/-y17PINUIlrM/Tj-A8VC-KMI/AAAAAAAALIk/6_BzkWeLQAE/qua_source.gif](https://lh3.googleusercontent.com/-y17PINUIlrM/Tj-A8VC-KMI/AAAAAAAALIk/6_BzkWeLQAE/qua_source.gif)
#### Вырезание ####
```php
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$src_x = 50; // точка начала вырезания по оси x
$src_y = 50; // точка начала вырезания по оси y
$crp_width = 200; // ширина вырезаемой области
$crp_height = 150; // высота вырезаемой области

if($croped_image  = ImagesHelper::crop($image_source, $src_x, $src_y, $crp_width, $crp_height)) {
   // сохранение полученного изображения в jpg формате  
   ImagesHelper::save($croped_image, $image_source,'crp_','jpg');    
}
```
![https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg](https://lh6.googleusercontent.com/-lOCc8X9-aT8/Tj9-ZeqF_bI/AAAAAAAALHs/2r-hSxCMcRo/source.jpg)
![https://lh5.googleusercontent.com/-MXMGr6p2qq0/Tj8RpPk9zdI/AAAAAAAALGo/uLRqCjkY1GE/crp_source.jpg](https://lh5.googleusercontent.com/-MXMGr6p2qq0/Tj8RpPk9zdI/AAAAAAAALGo/uLRqCjkY1GE/crp_source.jpg)

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>
