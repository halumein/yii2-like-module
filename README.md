Yii2-Like-module
==========
Модуль избранного для Yii2 фреймворка. ДЛЯ АВТОРИЗОВАННЫХ ПОЛЬЗОВАТЕЛЕЙ


Установка
---------------------------------
Выполнить команду

```
composer require halumein/yii2-like-module "*"
```

Либо в composer.json строку:

```
"halumein/yii2-like-module": "dev-master",
```


Далее, мигрируем базу:

```
php yii migrate --migrationPath=vendor/halumein/yii2-like-module/migrations
```

Подключение и настройка
---------------------------------
В конфигурационный файл приложения добавить модуль like

```php
    'modules' => [
        'like' => [
            'class' => 'halumein\like\Module',
        ],
        //...
    ]
```

Виджеты
==========
Кнопка-аналог лайков/рейтинга и т.д..

```php

<?php
use halumein\like\widgets\LikeButton;
?>

<?php /* Выведет кнопку поднатия рейтинга/лайка и т.д. */ ?>
<?= LiketButton::widget([
	'model' => $model
]) ?>


```

Дэфолтные css-стили
```css




```
