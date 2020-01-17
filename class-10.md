# Error Handling & Debugging

## Error Handling

JavaScript executes non-linearly, but with a easily traceable order of execution. Active code, like functions or conditionally executed logic, will only produce errors once it's called. Errors often arise when code calls on variables or functions that aren't defined yet, or defined within its scope.

When you get an error, it will show an error object in the console describing the type of error, helping you figure out if the issue is with syntax, invalid data types, or unknown variables. The console can usually be accessed from within your text editor, but is often better to view from your browser debugger. The error will show you a line number and (if possible) the specific code that is causing the issue. This should be enough to trace back the issue to whatever piece of code is the root of the problem.

If errors with variables become difficult to track, you can hunt bad or missing values by using `console.log(suspiciousVariable)`, or even just `console.log('check')` to check if the code is executing at all.

If you want to test your code piece by piece, or work with the first part of a code without getting to a buggy or incomplete later section, you can use breakpoints in your editor to stop the code at a set place, or to run through the code one piece at a time. This helps to compartmentalize the functionality of more complicated code.

Many errors can and should be handled gracefully in a way that allows the rest of the code to run. Sometimes simple errors might not have any noticeable effect on the functionality of the page. If a user occurs that blocks the user's progress, they can often fix the problem by reloading the page or trying an operation again.

You can also create your own errors to alert you to issues specific to your code's purpose by calling the `Error()` constructor function like so:

```js
if (answer < 0) {
  throw new Error('Negative number');
}
```

If you're running code that you expect might fail, you can account for failure states by using keywords that function similar to `if` and `else`. `try` will try to execute its following code, `catch` will run its code if the `try` code results in an error, and `finally` will run its code regardless of the previous outcomes.