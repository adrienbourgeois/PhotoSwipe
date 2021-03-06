PhotoSwipe
==========

A mobile photos gallery/browser.

This is a direct adaptation from the example presented in the demos of jquery.touchSwipe: [Imagegalleryexample.html](https://github.com/mattbryson/TouchSwipe-Jquery-Plugin/blob/master/demos/Image_gallery_example.html)

I modified the code to permit to have multiple galleries on the same page and to make it as easy as possible.

You can see a demo here: http://fathomless-waters-9473.herokuapp.com/

How to use it?
--------------

Include those files in your header:

    <link href="css/photos_gallery.css" rel="stylesheet" />
    <script src="javascript/jquery-2.0.3.min.js"></script>
    <script src="javascript/jquery.touchSwipe.min.js"></script>
    <script src="javascript/galleryPhotos.js"></script>

To create a new gallery, just put all your images inside those div blocks:

    <div id="content">
      <div class="imgs">
        <img src="...">
      </div>
    </div>

Update the listener after a DOM change
--------------------------------------

Let's say, for example, that you have ajax that update the content of the dom by adding a new gallery. To have the things working you just have to refresh the listener by calling: `listen_to_swipe()`
