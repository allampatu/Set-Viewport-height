# Set-Viewport-height
jQuery Function to calculate browser viewport for fullscreen

<code>

getWidthAndHeight();

// make sure div stays full width/height on resize
jQuery(window).resize(function() {
    getWidthAndHeight();
});

function getWidthAndHeight (){
    var winWidth = jQuery(window).width();
    var winHeight = jQuery(window).height();
    var headerHeight = jQuery('header').height(); 
    jQuery('.fullscreen').css({'width': winWidth,'height': winHeight - headerHeight,});
}

</code>
