---
title:       "Pan controls with Google Maps Javascript API v3.24+"
date:        2017-07-08 21:23:56
serie:       
category:    [ "Unaggregated" ]
tag:         [ "gist", "Google Maps" ]
---

As announced in the [Google Geo Developers Blog](https://maps-apis.googleblog.com/2015/09/new-controls-style-for-google-maps.html), pan controls are removed from the Google Javascript API since v3.24, which was released in February 2016.

The new panning controls are good and work especially well with mobile devices, but if you for any reason need the old panning control back, you can do it by creating your own custom control. This is relatively easy, but since it might not be trivial enough for everybody, here's how I solved the issue.

JavaScript
----------

In the script after initializing your map, add the following to create a new control wrapper:

`var panControl = document.createElement( 'div' );panControl.className = 'panControls';`

Next, we'll want to create the actual buttons for panning and add them to the control wrapper. Note: The code below refers to [pan\_arrow.png](https://open.knome.fi/files/2017/07/pan_arrow.png), which you need to provide – either download the one created by me or create your own instead. Alternatively, you can embed it in the script itself with base64; see the [gist](https://gist.github.com/knomepasi/aaeca1bd3b7499300f87ab072581858a) for an example.

```
var directions = ['North', 'West', 'East', 'South'];
var pan = [];
directions.forEach( function( item ) {
    pan[item] = document.createElement( 'div' );
    pan[item].className = 'panControl ' + item;
    pan[item].innerHTML = '<img src="pan_arrow.png" />';
    panControl.appendChild( pan[item] );
} );
```

After that, we'll add listeners for the buttons to activate panning on clicking. Change the panAmount variable (in pixels) to pan more or less per click.

```
var panAmount = 50;
pan['North'].addEventListener( 'click', function( ) {
    map.panBy( 0, -panAmount );
} );
pan['West'].addEventListener( 'click', function( ) {
    map.panBy( -panAmount, 0 );
} );
pan['East'].addEventListener( 'click', function( ) {
    map.panBy( panAmount, 0 );
} );
pan['South'].addEventListener( 'click', function( ) {
    map.panBy( 0, panAmount );
} );
```

Finally, we'll push the pan control wrapper to the left bottom of the map. Change LEFT\_BOTTOM to something else if you want to change the location of the panning control.

```
map.controls[google.maps.ControlPosition.LEFT_BOTTOM].push( panControl );
```

CSS
---

The JavaScript itself renders a not so good looking and mostly useless block of arrows all facing in the same direction even, so we'll need to add some CSS to go with it. Add the following CSS to your page with your map.

```
.panControls {
    position: relative;
    margin: 10px 20px;
    text-align: center;
    width: 40px;
    height: 40px;

    background-color: #fff;
    box-shadow: 0px 1px 4px -1px rgba( 0, 0, 0, 0.3 );
    border-radius: 2px;

    transform: rotate(-45deg);
}
    .panControls .panControl {
        width: 20px;
        height: 20px;
        -moz-user-select: none;
        cursor: pointer;
    }
        .panControl {
            position: absolute;
        }
            .panControl img {
                opacity: 0.6;
            }
                .panControl:active img {
                    opacity: 1;
                }
            .panControl.North {
                top: 0;
                left: 20px;
            }
            .panControl.West {
                top: 0;
                left: 0;
            }
                .panControl.West img {
                    transform: rotate( -90deg );
                }
            .panControl.East {
                top: 20px;
                left: 20px;
            }
                .panControl.East img {
                    transform: rotate( 90deg );
                }
            .panControl.South {
                top: 20px;
                left: 0;
            }
                .panControl.South img {
                    transform: rotate( -180deg );
                }

```

Now you have a nicer looking control that matches the style of the default controls!

Summary
-------

The panning controls you can create with the code above are very simple but serve my purpose very well. The above code can be found in a [gist](https://gist.github.com/knomepasi/aaeca1bd3b7499300f87ab072581858a).

There is at least one particular feature missing from these controls: constant panning when the buttons are held down for a longer time. The controls also do not include hover tooltips, let alone talking about localized ones.

Ultimately, you might want something completely different than I do, but I hope this can help you build the panning controls you need for your situation. Enjoy!
