# Javascript-setInterval

The `setInterval()` method allows us to run a function after a set period of time repeatedly.

```
const greet = () => console.log(`I've been instructed to greet you after every 3 seconds.`);

setInterval(greet, 3000);
/// This will run after every 3 seconds and not stop.
```

```
let annoyanceCount = 0;

const annoy = () => {
  annoyanceCount < 5
    ? (console.log(`I've been instructed to annoy you every second.`), annoyanceCount++)
    : clearInterval(annoyanceAlert);
};

const annoyanceAlert = setInterval(annoy, 1000);
/// This logic will run every second and stop after the fifth call
```

The `clearInterval()` method stops the periodic function calls set by the `setInterval()` method.
