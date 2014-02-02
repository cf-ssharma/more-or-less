#LESS CSS FUNCTIONS & MIXINS

...add some functions and mixins for lessjs

Auto prefixing css-properties should not be used.

It is advised to use libraries like 'autoprefixer'

Anyways.. if you want to use auto-prefixing mixins you can use the _css3.less file (also used in _images.less for .sprites-css3())

###Usage


    .border-radius {
        .border-radius(1px 2px 3px 4px;);
    }

    .box-shadow {
        .box-shadow(1px 0 2px rgba(0,0,0,0.3), 0 1px 2px rgba(255,0,0,0.3););
    }

    .box-sizing {
        .box-sizing(border-box);
    }

    .background-size {
        .background-size(10px auto, 100px auto;);
    }


    .sprite-right{
        .sprites('../img/sprite.png';
                 auto;
                 90px;
                 30;
                 one;
                 two;
                 three;);
    }

    .sprite-down{
        .sprites('../img/sprite.png';
                 90px;
                 auto;
                 30;
                 four;
                 five;
                 six;);
    }

    .calc {
        .calc(height;
              '100% - 10px');
        .calc(width;
              '50% - 20px');
    }

    .opacity {
        .opacity(0.4);
    }

    .text-overflow-ellipsis {
        .text-overflow(ellipsis);
    }

    .text-overflow-clip {
        .text-overflow(clip);
    }

    .transition-oneline {
        .transition(transform 200ms linear 400ms;);
    }

    .transition-separated {
        .transition-property(all);
        .transition-duration(200ms);
        .transition-timing-function(linear);
        .transition-delay(400ms);
    }

    .transition-prop-transform {
        .transition-property(transform;);
    }
    .transition-prop-mutli-with-transform {
        .transition-property(transform, color, height;);
    }

    .transition-prop-mutli-with-transform-and-boxShadow {
        .transition-property(transform, color, box-shadow;);
    }

    .transition-prop {
        .transition-property(height;);
    }
    .transition-multi {
        .transition-property(height, top, left;);
    }

    .transforms {
        .transform(translate(2px, 3px) rotate(3deg) scale(0.4));
    }
