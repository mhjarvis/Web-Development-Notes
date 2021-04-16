<h1 align=center>----- Fundamentals -----</h1>

# The Cascasde
Declarations can easily cause conflicts. The cascade considers three things to resolve issues:
1. Stylesheet origin - there are author styles (yours) and user agent styles (the browser's default). Yours take presedence. Agent styles often do things such s adding a margin to ```<h1>``` and ```<p>``` elements, or padding ```<li>``` elements.
    
    The !important declaration can overide presdence resulting in the following revised order:
    1. Author important
    2. Author
    3. User agent

3. Selector specificity - which selectors take precedence over which. This usually refers to inline styles (such as those included in the html tag) which will override any styles you apply in your stylesheet. 

4. Source order - order in which styles are declared in the stylesheet.
