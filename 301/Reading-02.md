# State and Props

## React Lifecycle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- According to the diagram, render happens first. 

2. What is the very first thing to happen in the lifecycle of React?

- The very first thing to happen in React is the instance creation. Nothing else can really proceed until the DOM has something to mount and work with. 

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- Constructor, Render, React Updates, componentDidMount, and finally componentWillUnmount. 

4. What does componentDidMount do?

- Allows us to execute the React code after the component is properly rendered. 


## React State vs. Props

* Props (properties) - Similar to arguments for a function when you create a component inside of React and when you want to Render it, you set the Props to enable your code to pass that through.
* State - From the video I understood this as the currently rendered data of your Component. 

1. What types of things can you pass in the props?

- Specific values that you need to be constant for your Component. 

2. What is the big difference between props and state?

- How they are handled in the component. Props are generated, written, or determined outside of the Component. State is always handled within the component.

3. When do we re-render our application?

- You re-render your application when you need to update or change the information being displayed. Or when the state has changed.

4. What are some examples of things that we could store in state?

- User Input, Check Box, Select Box, or other types of Data you will need to update or change on your component.

## Things I want to know more about

- How the guy from the video can explain so much in a 5 minute video. 

