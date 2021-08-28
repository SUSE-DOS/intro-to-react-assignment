[<img src="assets/images/su-logo.png" alt="Skills Union Logo" height="80px" />](https://www.skillsunion.com/)

# Intro to React: Assignment

## Brief

This assignment aims to help you practice what has been learned in the class independently.

Tasks:

1. You are to create a new project by the name `bulb-app`.
2. Add a new component file at `./bulb-app/src/components/bulb.js`.
3. Import `./src/components/bulb.js` component to `./bulb-app/src/App.js`.
4. In `bulb.js` file, copy and paste the follow code:

```js
import { useState } from "react";

function Bulb() {
  const [isOn, setIsOn] = useState(false);

  function toggle() {
    setIsOn(!isOn);
  }

  return (
    <>
      <span>Light Status: {isOn ? "On" : "Off"}</span>
      <br />
      <br />
      <button onClick={toggle}>Toggle</button>
    </>
  );
}

export default Bulb;
```

5. Run the react app using `npm run start` at the project root directory.
6. Browse http://localhost:3000
7. Click on "Toggle" button to see the value changes take place.
