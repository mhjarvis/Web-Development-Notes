<h1 align=center>----- Ruby Foundations -----</h1>

When talking about Ruby, _Ruby_ refers to the language itself, while _ruby_ refers to the interpreter. The _irb_ (interactive ruby console) is accessable via typing ```irb``` in the terminal. Using ```irb --simple-prompt``` is another option for a cleaner input prompt.

# Ruby Identifiers
The following make up the different identifier types found in Ruby:

1. **Variables** - 
    1. **Local** - variables use ```snake_case``` for variables, starting with lowercase or an underscore. Can include letters, underscores, and/or digits.
    2. **Instance** - variables that store information within individual objects always start with the ```@``` sign (e.g. ```@last_name```).
    3. **Class** - variables store information per class hierarchy; use double at-signs (e.g. ```@@running_total```).
    4. **Global** - variables start with a $ sign (e.g. ```$population``` or ```#FIRST_NAME```). 
2. **Constants** - begin with an uppercase letter (e.g. ```A```, ```String```, ```Pi```). The convention is to use either camel case or underscore-seperated all-uppercase words (e.g. ```FirstName``` or ```FIRST_NAME```).
3. **Keywords** - reserved words such as ```def```, ```class```, ```if```.
4. **Method** names - follow the same rules as local variables except that they can end with ```?```, ```!```, or ```=```.

### Running a Ruby Program
Ruby files are saved with the .rb ending. To run a file via the cmd line:

    ruby file-to-run.rb                         # runs file
    ruby -cw file-to-run.rb                     # checks for syntax error in code
    
### Printing (3 methods)
There are three main methods to print information: ```p```, ```puts```, and ```print```.

    p "Hello"           # prints string but also shows what type that string is
    puts "Hello"        # prints string but also add a newline character at the end
    print "Hello"       # prints string but does not add a newline

### Input and Output (I/O)
For user input we can use the ```gets``` command:

    puts "Enter your first name: "
    firstname = gets
    
To read data from a file in the directory:

    num = File.read("data-file.dat")            # reads file contents and assigns to num

To create a new file and write data to that file we can:

    new_string = "Hello there!"
    fh = File.new("temp.out", "w")              # create ne file and use the 'write' file mode (w)
    fh.puts new_string                          # print value to file
    fh.close                                    # 'fh' in this case is the write handle
    
### Loading External Files and Extensions
To facilitate breaking up programs into multiple files, Ruby provides the ```require``` and ```load``` methods. Remember that these are methods, and the ```load``` method will execute when the interpreter encounters that command during execution. The ```load``` method will always load the file asked for, whether it has been loaded before or not. This means if that file is changed, it will override aything in the original version. 
    
    load "second-ruby-file.rb"                  # load the secondary file
    load "../extraas.rb"                        # navigate relaaative directories in load commands
    
    load "/home/users/dblack/book/code/r.rb"    # force load using the direct path
    
One ofthe major differences of using ```require``` is that it will not reload a file if it has already been loaded. ```require``` is also more abstract, meaning you require a feature. Ruby also appends (for example) the .rb ending to the file name. ```require``` is the day-to-day technique that will be used most often. 

    require "./loadee"                          
    
##### require_relative
A final option to load files is to use the ```require_relative``` method. This command loads features by searching relative tot he directory in which the file from which it's called resides. 

    require_relative "loadee"                   # call without the current directory
    
    
    
    
    
