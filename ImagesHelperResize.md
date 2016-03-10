
# Изменение размера изображения #
При разработке различных программ очень часто приходится изменять размеры изображений, масштабировать и делать превьюшки. Ниже приведены несколько способов сделать с помощью класса ImagesHelper.

#### Масштабирование изображения ####
Изменение размера изображения масштабированием.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$ratio = 70; // соотношение в % от основного изображения
$prefix = 'sca_'; // Приставка к имени файла от масштабированного 
$format = 'gif'; // формат для сохранения изображения
   
if($scaled_image  = ImagesHelper::scale($image_source,$ratio)) {            
        // сохранение полученного изображения в gif формате            
        ImagesHelper::save($scaled_image, $image_source,$prefix,$format);     
}
```

#### Изменение размера изображения Пример 1 ####
Изменение размера изображения с выравниванием по ширине и масштабированием по высоте.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$new_width = 50; // фиксированная ширина будущего изображения в px
$prefix = 'thumb_'; // приставка к имени файла с измененными размерами 
$format = 'jpg'; // формат для сохранения изображения

if($resized_image  = ImagesHelper::resizeto($image_source,$new_width)) {
   // сохранение полученного изображения в jpg формате
   ImagesHelper::save($resized_image, $image_source,$prefix,$format);   
}
```
#### Изменение размера изображения Пример 2 ####
Изменение размера изображения с выравниванием по высоте и масштабированием по ширине.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$resize_to = 'height'; // фиксировать по высоте
$new_height = 30; // высота будущего изображения в px
$prefix = 'thumb2_'; // приставка к имени файла с измененными размерами 
$format = 'gif'; // формат для сохранения изображения

if($resized_image  = ImagesHelper::resizeto($image_source,$new_height,$resize_to)) {
   // сохранение полученного изображения в gif формате
   ImagesHelper::save($resized_image, $image_source,$prefix,$format);   
}
```

#### Изменение размера изображения Пример 3 ####
Изменение размера изображения без масштабирования и учета прежнего размера.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// Путь до файла картинки  
$image_source = './images/test.jpg'; 

$width  = 90; // ширина будущего изображения в px
$height = 30; // высота будущего изображения в px
$prefix = 'fix_'; // приставка к имени файла с измененными размерами 
$format = 'gif'; // формат для сохранения изображения

if($fix_resized_image  = ImagesHelper::resize($image_source,$width,$height)) {
   // сохранение полученного изображения в gif формате
   ImagesHelper::save($fix_resized_image, $image_source,$prefix,$format);   
}
```
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>