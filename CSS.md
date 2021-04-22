<h1 align=center>----- Fundamentals -----</h1>

# The Cascasde
Declarations can easily cause conflicts. The cascade considers three things to resolve issues:
1. Stylesheet origin - there are author styles (yours) and user agent styles (the browser's default). Yours take presedence. Agent styles often do things such s adding a margin to ```<h1>``` and ```<p>``` elements, or padding ```<li>``` elements. The !important declaration can overide presdence resulting in the following revised order:
    1. Author important
    1. Author
    1. User agent
2. Selector specificity - which selectors take precedence over which. This usually refers to inline styles (such as those included in the html tag) which will override any styles you apply in your stylesheet. Also, the number of selectors will also determine presedence. For example, ```main-nav a{}``` will have a higher priority than ```.feature```. Other things to note:
    1. IDs > Classes > Tags
    1. Specificities can be further determined by using the id,class,tag notation (0,0,0) depending on what selectors are used. Inline styles (if used) would add another line to the front of the notation.
3. Source order - order in which styles are declared in the stylesheet.

# Special Values
Two values can be applied to any property in the cascade: inherit and initital.
1. Inherit - It specifies that a property should inherit its value from its parent element.
2. Initial - resets a properties value to the default value.

<h1 align=center>----- Relative Units -----</h1>
CSS incorporates both absolute values (values that always mean the same thing (e.g. pixels)) and relative values (values that can change, based on external factors). 

# Relative Values
1. ```em``` - ```1em``` means the font size of the current element.This varies depending on the element it is being applied to.
