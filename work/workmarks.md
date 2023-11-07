## Разрешение экрана

**common.css**
#racer        { position: relative; z-index: 0; width: 1280px; height: 576px; margin-left: 0em; border: 2px solid black; }
#canvas       { position: absolute; z-index: 0; width: 1280px; height: 576px; z-index: 0; background-color: #72D7EE; }

**v4.final.html**
var width          = 1280;                    // logical canvas width
var height         = 576;                     // logical canvas height

## Атлас спрайтов

**v4.final.html** - game loop
images: ["background", "sprites", "sprotes_2"],

## Масщтаб всех спрайтов

**common.js**
SPRITES.SCALE = 0.3 * (1/SPRITES.PLAYER_STRAIGHT.w) // the reference sprite width should be 1/3rd the (half-)roadWidth - а так изначально
//SPRITES.SCALE = 0.3 * (1/80) - так я выравнял, но проблема с коллизиями