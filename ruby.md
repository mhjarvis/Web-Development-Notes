<h1 align=center>----- Fundamentals -----</h1>

# Printing
  
    print                   # minimal formating; does not add a new line
    puts                    # adds new line after every 'puts'
    p                       # prints data, adds newline, and shows the type of data that was printed
    
# Methods

    def someMethod(var1, var2)
      # code
      # code
      return x
    end
    
    someMethod              # or someMethod()

# Conditionals

    num = 0
    
    if num > 0
      puts 'positive'
    elsif num < 0
      puts 'negative'
    else
      puts 'zero'
    end

# Looping

    count = 0
    
    whitle count < 5
      puts counter
      counter += 1
    end
    
# Enumerable Methods

    people = ["John", "Mike", "Lee"]
    
    people.each { |person| puts person }                # prints each name in the array
    
    people.each_with_index do |person, i|               # prints name, index, and dashes
      puts person
      puts i
      puts "-----"
    end
    
# String Enumerable Methods

    greeting = "Hello"
    
    greeting.each_char { |char| puts chara }            # prints each letter
    
    greeting.each_char.with_index do |chr, i|           # print letter, index, and dashes
      puts char
      puts i
      puts "-----"
    end
    
# Other Enumerables

    3.times do                      # prints 'hi' three times
      puts 'hi'
    end
    
    (2..6).each {|n| puts n}        # prints numbers 2-6
    (2...6).each {|n| puts n}       # prints 2-5
    
