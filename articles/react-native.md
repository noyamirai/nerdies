# An Introduction to React Native for Beginners

Starting september, I will be doing my senior internship at Triple as a React Native developer. I have plenty of experience in regards of web development (vanilla HTML/CSS/JS, Node.js, PHP, MySQL, a little bit of React) and even iOS development, but React Native is completely new to me! I wanted a challenge, so I felt React Native would give me that challenge. However, since I am a React Native newbie, I wanted to write an introduction about React Native for other beginners like me!

I have worked in the app development department before, iOS development to be specific, and we would work together with the Android development team. Two different teams, two different languages all for the sake of native mobile development! In Android development, you write views in Kotlin or Java; in iOS development, you use Swift or Objective-C. With React Native, you can invoke these views with JavaScript using React components. React Native provides an accessible and efficient way to create stunning cross-platform mobile applications.

## Understanding React Native

React Native is an open-source framework developed by Facebook that allows developers to build native mobile applications using JavaScript and React. It takes advantage of the React library's component-based architecture, enabling developers to write code once and deploy it across multiple platforms, including iOS and Android. What does this mean? Well, now web developers can also create mobile applications that look and feel truly “native,” all from the comfort of a JavaScript library. This approach saves time and effort, as developers no longer need to build separate codebases for each platform, as I mentioned before.

Similar to React, React Native applications are written using a mixture of JavaScript and JSX. Then, React Native “bridge” invokes the native rendering APIs in Objective-C (for iOS) or Java (for Android). This means your application will render using real mobile UI components, delivering a native-like user experience with smooth animations, gestures, and performance, giving users an app that feels just like a native one.

In Android and iOS development, a **view** is the basic building block of UI: a small rectangular element on the screen which can be used to display text, images, or respond to user input. Even the smallest visual elements of an app, like a line of text or a button, are kinds of views.

### Core Concepts of React Native

- **Components:** React Native is built on the concept of reusable components, such as `<View>` or `<Text>`, which are self-contained pieces of code that encapsulate specific functionalities and UI elements. Components can be combined to create complex user interfaces, making the development process modular and efficient.
- **JSX:** React Native uses JSX (JavaScript XML) syntax, an extension of JavaScript that allows developers to write HTML-like code within their JavaScript files. This makes it easier to define and manipulate the user interface components in a declarative manner
- **Virtual DOM:** React Native utilizes a virtual representation of the app's user interface called the Virtual DOM. It efficiently updates only the necessary components when changes occur, resulting in improved performance and a smoother user experience

### States and Hooks

States in React are used to manage and store data that can change over time within a component. Think of a state as a container or localstorage for storing and updating information that affects how your component renders and behaves. For example, if you have a counter component, the current count value can be stored in a state. When a state value changes, React automatically re-renders the component to reflect the updated state. Hooks are functions in React that allow you to use state and other React features in functional components. Before hooks were introduced, state management was primarily done in class components. Hooks provide a more straightforward and concise way to handle state in functional components.

**useState Hook:** 
The useState hook is the most commonly used hook for managing state in React. It enables you to add state to a functional component without converting it to a class component. Here's a simple example:

```js
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0); // Initial value is 0

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}
```

In the example above, the `count` variable represents the state, and `setCount` is the function to update the state. The `useState(0)` hook call sets the initial value of `count` to 0. When the button is clicked, the `setCount` function is called to increment the count value, triggering a re-render. React provides several other hooks that serve specific purposes, such as:

- **useEffect:** It allows you to perform side effects, like data fetching, when certain dependencies change.
- **useContext:** It enables you to access and use the value from a React context.
- **useRef:** It provides a way to reference a mutable value that persists across renders.
- **useReducer:** It is an alternative to useState when managing more complex state logic.

And that's it for my React introduction. Obviously there is A LOT more to it, but at this point, you should just try it out for yourself if you find it interesting!

## Resources

- [React Native](https://reactnative.dev/)
- [React Fundamentals](https://reactnative.dev/docs/intro-react)
- [Chapter 1. What Is React Native?](https://www.oreilly.com/library/view/learning-react-native/9781491929049/ch01.html)