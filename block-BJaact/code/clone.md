1. Write the output with reason

```js
const person = {
  firstName: 'John',
  lastName: 'Doe',
};

let person2 = person;

person.firstName = 'Arya';

console.log(person2.firstName); // output
console.log(person.firstName); // output
console.log(person.lastName); // output
console.log(person == person2); // output
console.log(person === person2); // output
console.log(person.lastName === person2.lastName); // output
```

2. Write the output with reason

```js
const person = {
  firstName: 'John',
  lastName: 'Doe',
};

let person2 = { ...person };

person.firstName = 'Arya';

console.log(person2.firstName); // output
console.log(person.firstName); // output
console.log(person.lastName); // output
console.log(person == person2); // output
console.log(person === person2); // output
console.log(person.lastName === person2.lastName); // output
```

3. Write the output with reason:

```js
let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let personTwo = { ...person };

person.firstName = 'Arya';
person.city = 'Navada';

console.log(personTwo.firstName); // output
console.log(person.firstName); // output
console.log(personTwo.lastName); // output
console.log(person.firstName === personTwo.firstName); // output
console.log(person == personTwo); // output
console.log(person === personTwo); // output
console.log(person.address === personTwo.address); // output
console.log(person.address == personTwo.address); // output
console.log(personTwo.address.city); // output
console.log(person.address.city); // output
console.log(person.address.city == personTwo.address.city); // output
```

4. Write the output with reason:

```js
let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let personTwo = { ...person, address: { ...person.address } };

person.firstName = 'Arya';
person.city = 'Navada';

console.log(personTwo.firstName); // output
console.log(person.firstName); // output
console.log(personTwo.lastName); // output
console.log(person.firstName === personTwo.firstName); // output
console.log(person == personTwo); // output
console.log(person === personTwo); // output
console.log(person.address === personTwo.address); // output
console.log(person.address == personTwo.address); // output
console.log(personTwo.address.city); // output
console.log(person.address.city); // output
console.log(person.address.city == personTwo.address.city); // output
```

5. Clone the `blogs` variable into a new variable named `clonedBlogs`

```js
let blogs = [
  {
    id: 1,
    title: 'Post #1',
    body: 'My first blog post',
  },
  {
    id: 2,
    title: 'Post #2',
    body: 'My second blog post',
  },
  {
    id: 3,
    title: 'Post #3',
    body: 'My third blog post',
  },
];

// Your code goes here
```

6. Clone the `question` variable into a new variable named `questionClone`

```js
var questions = [
  {
    prompt: 'Why is the sky blue?',
    responses: [
      'Because the color blue was on sale at Wallmart',
      'Because blue is the prettiest color',
      'Because the air molecules difract blue light more than any other color',
    ],
  },
  {
    prompt: 'Why are leaves usually green?',
    responses: [
      'So green caterpillars can hide better.',
      'Because leaves can more easily make energy with green light',
      "Because leaves absorb red and blue light so it's green that is reflected",
    ],
  },
];

// Your code goes here
```

7. Clone the `allBlogs` variable into a new variable named `allBlogsClone`

```js
var allBlogs = {
    id: 1,
    title: "Alamofire JSON Serialization",
    body: "All about serialization in Alamofire...",
    author: {
        id, 1,
        fullName: "Jeff Potter",
        username: "jpotts18"
    },
    comments: [
        {
          id: 1,
          body: "Thanks for the help Jeff, this saved me hours"
        },
        {
          id: 2,
          body: "Your welcome. I am happy to help!"
        }
    ]
}

// Your code goes here
```

8. Clone the `person` variable into a new variable named `clonedPerson`

```js
let person = [
  {
    input: { name: 'Ryan' },
    output: { name: 'Ryan' },
  },
  {
    input: { name: { first: 'Ryan', last: 'Haskell-Glatz' } },
    output: { firstName: 'Ryan', lastName: 'Haskell-Glatz' },
  },
  {
    input: { name: 'Ryan', age: 24 },
    output: { name: 'Ryan', age: 24 },
  },
  {
    input: {
      name: { first: 'Ryan', last: 'Haskell-Glatz' },
      birthday: { year: 1993, month: 'Nov' },
    },
    output: {
      firstName: 'Ryan',
      lastName: 'Haskell-Glatz',
      birthdayYear: 1993,
      birthdayMonth: 'Nov',
    },
  },
];

// Your code goes here
```

9. Write a function named `cloneObject` that accepts an object and returns the clone of the object

```js
function cloneObject() {
  // your code
}

// Run the test below to check your function

let user = {
  name: 'John',
  house: 'Stark',
  sisters: ['Arya', 'Sansa'],
};
let cloned = cloneObject(user);

let person = {
  firstName: 'John',
  lastName: 'Doe',
  address: {
    street: 'North 1st',
    city: 'San Jose',
    state: 'CA',
    country: 'USA',
  },
};

let clonedPerson = cloneObject(user);

console.log(
  `The user object is ${
    user == cloned ? `not clone` : `cloned successfully 😁👑`
  }`
);
console.log(
  `The person object is ${
    person == clonedPerson ? `not clone` : `cloned successfully 😁👑`
  }`
);
```
