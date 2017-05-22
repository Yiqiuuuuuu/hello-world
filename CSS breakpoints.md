# Seriously, how many Media Query breakpoints should I put in css?? 

**In Bootstrap**http://getbootstrap.com/css/, they use the following media queries in their Less files to create the key breakpoints in their grid system:

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


I also found an image in **David Gilbertson's** https://medium.freecodecamp.com/the-100-correct-way-to-do-css-breakpoints-88d6a5ba1862 article presenting different screen sizes with commonly-used breakpoints name like "portrait tablet":

![Image of different screen sizes](pics/screenSizes.png)

