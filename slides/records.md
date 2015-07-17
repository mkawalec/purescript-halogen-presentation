##  Records

compile to javascript objects

    data Person = Person { name :: String, age :: Number }

    examplePerson :: Person
    examplePerson = Person { name: "Bonnie", age: 26 }


    var Person = (function () {
      function Person(value0) {
          this.value0 = value0;
      };
      Person.create = function (value0) {
          return new Person(value0);
      };
      return Person;
    })();
    var examplePerson = new Person({
        name: "Bonnie",
        age: 26
    });
