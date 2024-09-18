<div align="center">
  <img height="60" src="https://dabeng.github.io/img/reactjs.png">
  <h1>ReactJS Interview Questions</h1>
</div>

> [!NOTE]  
> This repository was created in 2024, and the questions here reflect the ReactJS syntax and practices of that time. As both React and JavaScript continue to evolve, newer features and changes may not be covered in the questions provided. It’s recommended to stay updated with the latest React and JavaScript documentation.

<p align="center">
From basic to advanced: test how well you know ReactJS, refresh your knowledge, or prepare for your coding interview! :muscle: :rocket: I update this repository regularly with new questions. Answers are provided in the collapsed sections below each question—just click to expand them. Have fun and good luck! :heart:</p>

###### 1. What is ReactJS?
 
ReactJS, also known as React, is a popular JavaScript library for building user interfaces. It is also referred to as a front-end JavaScript library. It was developed by Facebook and is widely used for creating dynamic and interactive web applications. In this article, we’ll explore the key concepts of React.

**How to Use Refs:**
1. **Create a Ref:** You can create a ref using `React.createRef()` or with a callback function.
2. **Attach the Ref:** Attach the ref to a DOM element or React component via the `ref` attribute.
3. **Access the Ref:** Access the ref via `this.refs` in class components or `ref.current` in functional components.

**Example:**

```jsx
import React, { useRef, useEffect } from 'react';

const MyComponent = () => {
  const inputRef = useRef(null);

  useEffect(() => {
    inputRef.current.focus();  // Focus on the input field when the component mounts
  }, []);

  return (
    <div>
      <input type="text" ref={inputRef} />  {/* Assigning ref */}
    </div>
  );
};

export default MyComponent;




