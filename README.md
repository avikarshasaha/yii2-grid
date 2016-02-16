Custom Grid
===========
Grid

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist avikarsha/yii2-grid "*"
```

or add

```
"avikarsha/yii2-grid": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?php 
use avikarsha\grid\GridView;

<?= GridView::widget([
        'dataProvider' => $dataProvider,
        'summary' => '<div class="css-group-head"><i class="css-groups-sign-box">r</i>Retail</div>',
        'columns' => [
            ['class' => 'yii\grid\SerialColumn'],
            ...
        ],
        'options'=>['class'=>'css-manage-group-table']
    ]); ?>
?>```