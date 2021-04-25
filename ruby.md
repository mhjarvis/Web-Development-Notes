<h1 align=center>----- Ruby Foundations -----</h1>

When talking about Ruby, _Ruby_ refers to the language itself, while _ruby_ refers to the interpreter. The _irb_ (interactive ruby console) is accessable via typing ```irb``` in the terminal. Using ```irb --simple-prompt``` is another option for a cleaner input prompt.

# Ruby Identifiers
The following make up the different identifier types found in Ruby:

1. Variables - 
    1. Local - variables use ```snake_case``` for variables, starting with lowercase or an underscore. Can include letters, underscores, and/or digits.
    2. Instance - variables that store information within individual objects always start with the ```@``` sign (e.g. ```@last_name```).
    3. Class - variables store information per class hierarchy; use double at-signs (e.g. ```@@running_total```).
    4. Global - variables start with a $ sign (e.g. ```$population``` or ```#FIRST_NAME```). 
2. Constants - begin with an uppercase letter (e.g. ```A```, ```String```, ```Pi```). The convention is to use either camel case or underscore-seperated all-uppercase words (e.g. ```FirstName``` or ```FIRST_NAME```).
3. Keywords - reserved words such as ```def```, ```class```, ```if```.
4. Method names - follow the same rules as local variables except that they can end with ```?```, ```!```, or ```=```.
