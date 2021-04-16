<h1 align=center>----- Fundamentals -----</h1>

# Object Literals
Objects are containers that hold values combined to form a single data structure that has a particular identity. The data is calld properties and are represented by pairs of names and values. The functionalities are called methods and are represented by functions. 

    let emptyObject = {};                                   //empty object
    let person = {name: "John", "suname": "Smit"};          //object with values
    let person = {"first-name": "John"};                    //quotes are optional unless the name does not follow normal variable rules

## Property Access
Properties can be accessed by dot-notation or using square brackets.

    let person = {
                name: "John",
                surname: "Smith",
                address: {
                    street: "103 Main Street",
                    city: "Salt Lake City"
                }
    }
    
    console.log(person.address.street);                     //'103 Main Street'
    console.log(person["name"]);                            //'John'
    console.log(person["address"]["city"]);                 //'Salt Lake City'
    
    
    
