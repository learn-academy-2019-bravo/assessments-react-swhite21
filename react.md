# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React is a modern, efficient answer to complex UI applications
- React is a flexible library that plays the role of V in an MVC framework


 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.



 //Your Answer
smart components contain logic or "instructions" whereas dumb components are essentially static and have no built in logic.

 //Googled Answer
Dumb components are also called ‘presentational’ components because their only responsibility is to present something to the DOM
Smart components (or container components) on the other hand have a different responsibility. Because they have the burden of being smart, they are the ones that keep track of state and care about how the app works.


#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?


 //Your Answer
yarn add ... will add a package like bootstrap to your react-project project. this will update your local repository.

 //Googled Answer
 In general, a package is simply a folder with code and a package.json file that describes the contents. When you want to use another package, you first need to add it to your dependencies. This means running yarn add [package-name] to install it into your project.

This will also update your package.json and your yarn.lock so that other developers working on the project will get the same dependencies as you when they run yarn or yarn install.


#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

    import React, { Component } from 'react';

    class Recipes extends Component{
      constructor(props){
        super(props)
        this.state = {
          recipes:
            {name: 'Meatballs',
            name: 'Mac & Cheese'}

        }
      }

      render() {
        const {recipes}=this.state

        return (

          let recipes = recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })

          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
number, email, and checkbox

 //Googled Answer
 <input type="button">
 <input type="checkbox">
 <input type="color">

 #### 7. How would you explain state to a friend who doesn't know code?
 //Your Answer
 state is like the code taking a snapshot of its configuration or current values to be used or referenced at a later point.


 //Googled Answer
The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behaviour of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component

 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer
State as mentioned above, holds a value in a key-value pair and can be called in the component it is set in by simply using this.state.mystate. a prop is similar to state but the main difference is props are declared in a parent component then passed as a prop to the child.

 //Googled Answer
Props and state are related. The state of one component will often become the props of a child component. Props are passed to the child within the render method of the parent as the second argument to React.createElement() or, if you're using JSX, the more familiar tag attributes.

#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
