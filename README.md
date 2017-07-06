Owl Carousel Widget 2
============================

The OwlCarouselWidget is a Yii2 wrapper for the [Owl Carousel 2] (https://owlcarousel2.github.io/OwlCarousel2/)

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist kv4nt/yii2-owl-carousel2 "*"
```

or add

```
"kv4nt/yii2-owl-carousel2": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
use kv4nt\owlcarousel\OwlCarouselWidget;

OwlCarouselWidget::begin([
    'container' => 'div',
    'containerOptions' => [
        'id' => 'container-id',
        'class' => 'container-class'
    ],
    'pluginOptions' => [
        'autoPlay' => 3000,
        'items' => 2,
        'itemsDesktop' => [1199,3],
        'itemsDesktopSmall' => [979,3]
    ]
]);

<div class="item-class"><img src="/img/1.jpg" alt="Image 1"></div>
<div class="item-class"><img src="/img/2.jpg" alt="Image 2"></div>
<div class="item-class"><img src="/img/3.jpg" alt="Image 3"></div>
<div class="item-class"><img src="/img/4.jpg" alt="Image 4"></div>


OwlCarouselWidget::end();
