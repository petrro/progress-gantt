<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [ProgressGantt][1]
    -   [Parameters][2]
    -   [draw][3]
        -   [Parameters][4]
    -   [remove][5]
    -   [imageSource][6]
    -   [svgSource][7]

## ProgressGantt

<a href='https://travis-ci.com/ulfschneider/progress-gantt'><img src='https://travis-ci.com/ulfschneider/progress-gantt.svg?branch=master'/></a>
<a href='https://coveralls.io/github/ulfschneider/progress-gantt?branch=master'><img src='https://coveralls.io/repos/github/ulfschneider/progress-gantt/badge.svg?branch=master' /></a>
<a href='https://badge.fury.io/js/progress-gantt'><img src='https://badge.fury.io/js/progress-gantt.svg' /></a>

Draw a progress gantt.

<img src="https://github.com/ulfschneider/progress-gantt/blob/master/progress-gantt.png?raw=true"/>

Play with the settings of the progress-gantt by visiting the [progress-gantt playground][8].

Install in your Node project with 

<pre>
npm i progress-gantt
</pre>

and use it inside your code via 

<pre>
const progressGantt = require('progress-gantt');
</pre>

or, alternatively 

<pre>
import progressGantt from 'progress-gantt';
</pre>

Create the new progress gantt objects via

<pre>
let diagram = progressGantt(settings);
</pre>

### Parameters

-   `settings` **[Object][9]** The configuration object for the progress gantt. 
    All data for the progress gantt is provided with this object.
    -   `settings.svg` **[Object][9]** The DOM tree element, wich must be an svg tag.
        The progress gantt will be attached to this DOM tree element. Example:<pre>settings.svg = document.getElementById('progressGantt');</pre><code>'progressGantt'</code> is the id of a svg tag.
    -   `settings.id` **[String][10]?** The id of a domtree svg element, to which the progress gantt will be bound to. 
        The id will only be used in case settings.svg is not provided.
    -   `settings.width` **[Number][11]?** Width in pixels for the progress gantt without borders and margins. Default is <code>600</code>.
    -   `settings.height` **[Number][11]?** Height in pixels for the progress gantt without borders and margins. Default is <code>400</code>.
    -   `settings.fontSize` **[Number][11]?** Size in pixels for all labels. Default is <code>16</code>
    -   `settings.fontFamily` **[String][10]?** The font to use for all labels. Default is <code>sans-serif</code>.
    -   `settings.margin` **{top: [Number][11], right: [Number][11], bottom: [Number][11], left: [Number][11]}?** The margin for the progress gantt. 
        Default values are:<pre>settings.margin = {
        top: 0,
        right: 0,
        bottom: 0,
        left: 0 }
        </pre>

### draw

Draw the progress gantt.

#### Parameters

-   `settings` **[Object][9]?** The configuration object for the progress gantt. Optional.
    If provided, will overwrite the settings object already given to the constructor.

### remove

Clear the progress gantt.

### imageSource

Draw the progress gantt and return the result as a string which can be assigned to the SRC attribute of an HTML IMG tag.

Returns **[string][10]** 

### svgSource

Draw the progress gantt and return the result as a SVG tag string.

Returns **[string][10]** 

[1]: #progressgantt

[2]: #parameters

[3]: #draw

[4]: #parameters-1

[5]: #remove

[6]: #imagesource

[7]: #svgsource

[8]: https://htmlpreview.github.io/?https://github.com/ulfschneider/progress-gantt/blob/master/progress-gantt-playground.html

[9]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[10]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[11]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number
