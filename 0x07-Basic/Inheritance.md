# Inheritance
Inheritance is a fundamental concept in object-oriented programming (OOP) that allows a class to inherit properties and methods from another class.
Inheritance helps avoid code duplication when multiple classes share common behavior.

```js
class Animal {
  constructor(numLegs, numEyes) {
    this.numLegs = numLegs;
    this.numEyes = numEyes;
  }

  move() {s
    console.log(`Animal looking at the road with ${this.numEyes} eyes`);
    console.log(`Animal moving with ${this.numLegs} legs`);
  }

  eat() {
    console.log(`Animal eating for survival`);
  }
}

class Cow extends Animal {
  constructor(numLegs, numEyes, breed, gender) {
    super(numLegs, numEyes); // calls the parent constructor
    this.breed = breed;
    this.gender = gender;
  }

  sound() {
    console.log(`The ${this.gender} ${this.breed} cow is mooing`);
  }
}

const myCow = new Cow(4, 2, "Guernsey", "Male");
myCow.move();
myCow.eat();
myCow.sound();