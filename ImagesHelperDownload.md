
# Скачивание изображения #
Этот пример полезен, если вам нужно загрузить изображения с удаленного компьютера.
```
// Подключение класса 
require_once 'class.images.helper.php'; 

// локальный путь для сохранения изображений
$destination_path = './images/'; 
// путь к удаленному источнику изображения
$image_url = 'http://agjoomla.com/media/k2/categories/1.png'; 

// загрузка изображения с удаленного сервера
$image_source = ImagesHelper::download($image_url,$destination_path);
```
#### [Скачать класс](http://code.google.com/p/ag-php-classes/downloads/list)  [Исходный код](http://code.google.com/p/ag-php-classes/source/browse/#svn%2Ftrunk%2FImages) ####

---

<span>
<a href='http://www.gordejev.lv/'><img src='http://www.gordejev.lv/templates/gordejev/images/gora_88x31.png' /></a>
<br />
</span>