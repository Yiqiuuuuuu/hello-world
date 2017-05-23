# Seriously, how many Media Query breakpoints should I put in css:question::question::question:

[**In Bootstrap**](http://getbootstrap.com/css/), they use the following media queries in their Less files to create the key breakpoints in their grid system:

    /* Extra small devices (phones, less than 768px) */
    /* No media query since this is the default in Bootstrap */
    
    /* Small devices (tablets, 768px and up) */
    @media (min-width: @screen-sm-min) { ... }
    
    /* Medium devices (desktops, 992px and up) */
    @media (min-width: @screen-md-min) { ... }
    
    /* Large devices (large desktops, 1200px and up) */
    @media (min-width: @screen-lg-min) { ... }

They occasionally expand on these media queries to include a max-width to limit CSS to a narrower set of devices:

    @media (max-width: @screen-xs-max) { ... }
    @media (min-width: @screen-sm-min) and (max-width: @screen-sm-max) { ... }
    @media (min-width: @screen-md-min) and (max-width: @screen-md-max) { ... }
    @media (min-width: @screen-lg-min) { ... }



I also found a pretty good image in [**David Gilbertson's** ](https://medium.freecodecamp.com/the-100-correct-way-to-do-css-breakpoints-88d6a5ba1862) article presenting different screen sizes with commonly-used name like "portrait tablet":laughing::

![Image of different screen sizes](pics/screenSizes.png)

Like Josh Brewer said:

> If you think responsive's simple, I feel bad for you son. We got 99 viewports, but the iPhone's just one.
> - —[Josh Brewer, March 10, 2010](https://twitter.com/jbrewer/status/178528003402379265)

In the market, there are various screen views. If I add breakpoints for every single screen size, this woulb be a little bit overwhelming.

There is a point of view I feel like to be a good solution and it seems to be approved by plenty of people (an answer on [stact overflow](https://stackoverflow.com/questions/16443380/common-css-media-queries-break-points)):
> Rather than try to target @media rules at specific devices, it is arguably more practical to base them on your particular layout instead. That is, gradually **narrow your desktop browser window and observe the natural breakpoints for your content**. It's different for every site. **As long as the design flows well at each browser width, it should work pretty reliably on any screen size** (and there are lots and lots of them out there.)



