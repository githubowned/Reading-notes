# Read: Class 04 - Readings: React and Forms

## What is a controlled component ?
 - A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange . A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component.

<p>&nbsp;</p>

 - In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

<p>&nbsp;</p>

 ```js 
 class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}

```
<p>&nbsp;</p>
<p>&nbsp;</p>

## The Conditional (Ternary) Operator Explained

> Shorten your `if` statements into one line of code with the conditional operator

Example: 
```js 
let person = {
  name: 'tony',
  age: 20,
  driver: null
};
```
- Now I want to  change the driver value to yes or no based on  his age.

```js
if (person.age >= 16) {
  person.driver = 'Yes';
} else {
  person.driver = 'No';
}
```

> we can write the previous code by one line!
```js
person.driver = person.age >=16 ? 'Yes' : 'No';
```

```js
condition ? value if true : value if false
```

another example:
- theatre fees for non students 12$
- theatre fees for students 8$

```js
let isStudent= true ? '8' : '12'
```
<p>&nbsp;</p>
<p>&nbsp;</p>
===========================================

- Answering questions:
1. What is a ‘Controlled Component’?answered in the definition.
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why. answered in the definition
3. How do we target what the user is entering if we have an event handler on an input field? answered in the example
-----------------------------------------------------------

- answering the second part:
Why would we use a ternary operator?- Shorten your `if` statements into one line of code with the conditional operator

Rewrite the following statement using a ternary statement:

  ```js 
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```
answer code: 

```js
let answer =((x===y) ? 'true': 'false');
```





References:

---
1. [React Docs - Forms](https://reactjs.org/docs/forms.html)
2. [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
3. [React Bootstrap - Forms](https://react-bootstrap.github.io/components/forms/)
4. [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)

