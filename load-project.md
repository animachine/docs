# Load Project

The project file is an UMD module so you can import it in any kind of js app.
> The following example is using CommonJS with ES5 syntax but for example you could load the project file with a script tag and get the project as a global js object.


```javascript
var myProject = require('./myProject.am.js')
var node = document.getElementById('anim-root')
var timeline = myProject.timelineName(node)
```
> **Note:** One Project can contain many Timelines

The created timeline is a [GSAP TimelineMax](https://greensock.com/timelinemax) instance. Check out its [API](https://greensock.com/docs/#/HTML5/GSAP/TimelineMax/) to see how you can controll it.

```javascript
//example
timeline.pause()
timeline.resume()
timeline.seek(1.5)
timeline.reverse()
```

> ###### [Save Project](save-project.md)
