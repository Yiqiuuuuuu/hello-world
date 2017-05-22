# Seriously, how many CSS Media Query breakpoints shou I make?? 

**In Bootstrap**, they use the following media queries in their Less files to create the key breakpoints in their grid system:

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


While I was 
![Image of different screen sizes](pics/screenSizes.png)

