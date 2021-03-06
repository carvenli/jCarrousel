# jCarrousel

A jQuery Plugin to make a powerful 3D slider

----

## Introduction

Based on [`jquery.gallery.js`](http://tympanus.net/codrops/2012/02/06/3d-gallery-with-css3-and-jquery/) from `Pedro Botelho`

[详情及中文说明](http://www.anotherhome.net/2063)

[Demo](http://www.anotherhome.net/file/jCarrousel)

## How it works

The following HTML structure is used for the carrousel:


```
<div class="banner">
    <section id="dg-container" class="dg-container">
        <div class="dg-wrapper">
            <a href="#" link="http://www.anotherhome.net">
                <img src="images/1.jpg">
            </a>
            <a href="#" link="http://www.anotherhome.net">
                <img src="images/2.jpg">
            </a>
            <!-- ... -->
        </div>
        <ol class="button" id="lightButton">
            <li index="0">
            <li index="1">
            <!-- ... -->
        </ol>
        <nav>
            <span class="dg-prev"></span>
            <span class="dg-next"></span>
        </nav>
    </section>
</div>
```

And this is how the carrousel is initialized:

```
$('#dg-container').carrousel({
    current: 0,
    autoplay: true,
    interval: 3000
});
```

## Options

The following options are available:

```
// index of current item
current		: 0,

// slideshow on / off
autoplay	: false,

// time between transitions
interval	: 2000
```

## API

+ `$('#dg-container').carrousel('play');` -- play
+ `$('#dg-container').carrousel('stop');` -- stop
+ `$('#dg-container').carrousel('next');` -- switch to the next picture
+ `$('#dg-container').carrousel('prev');` -- switch to the previous picture
+ `$('#dg-container').carrousel(3);`      -- switch to the fourth picture

## License

Free to use under the MIT license.