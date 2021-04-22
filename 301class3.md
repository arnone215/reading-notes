# 301 reading notes 3


Lifting State Up
Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor. Let’s see how this works in action.

Writing Conversion Functions
First, we will write two functions to convert from Celsius to Fahrenheit and back:

`function toCelsius(fahrenheit) {
  `return (fahrenheit - 32) * 5 / 9;
`}

`function toFahrenheit(celsius) {
  `return (celsius * 9 / 5) + 32;
`}
These two functions convert numbers. We will write another function that takes a string temperature and a converter function as arguments and returns a string. We will use it to calculate the value of one input based on the other input.

In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”. We will remove the local state from the TemperatureInput and move it into the Calculator instead.

If the Calculator owns the shared state, it becomes the “source of truth” for the current temperature in both inputs. It can instruct them both to have values that are consistent with each other. Since the props of both TemperatureInput components are coming from the same parent Calculator component, the two inputs will always be in sync.

resource - https://reactjs.org/docs/lifting-state-up.html