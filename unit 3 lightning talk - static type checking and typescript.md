# Static Type Checking and TypeScript

By: Lux Barker (they/them)

---

##### first off, what the hecking is "static type checking"

- JavaScript and Python are both "dynamically" typed --> you don't have to tell them manually what type a variable is
- if you do this:

	```js
	const msg = "hello";
	```

- when the the JavaScript engine reads this line, it sees that you gave it a string, and assigns `msg` a type of `string` all on its own
- a statically typed language is where you actually write out in your code what the type of a variable is yourself; you stop letting the interpreter make its own decisions

---

##### enter TypeScript

- TypeScript is a statically typed *superset* of JavaScript
	- Basically its extra fancy syntactical sugar on top of JavaScript
	- Any valid JavaScript code is already valid TypeScript code; its features are fairly opt-in
- developed by Microsoft
- with the `tsc` compiler, it compiles down to standard JavaScript code that can run in the browser

---

##### ok but if JavaScript can figure out types on its own, what's the point??

- because TypeScript has a compilation phase where it gets parsed down into regular JavaScript, its helpful in catching bugs that you might otherwise have missed
- for example if you had the lines:
	```js
	const me = "tired";
	tired();
	```
- JavaScript would let you run the file and then present you with an error during runtime
- TypeScript however would alert you during the compiling phase before you ever run it and let you know you messed up!
- what's also nice is that TypeScript knows about JavaScript's implied typing; you don't have to manually set `msg` to a string type here. Assigning the variable is enough.

---

##### cool uses

- defining a shape for objects:

	```ts
	interface Person {
		name: string,
		energyLevel: number
	};

	// which you can use like this:
	const me: Person = {
		name: 'Lux',
		energyLevel: 0
	};
	// if I didn't include both name and energyLevel (or if they were the wrong types), we'd get an error during compile
	```

- annotate parameters and return values:

	```ts
	function checkEnergy(person: Person): number { // this means person should be of type Person and the func should return a number!
		return person.energyLevel;
	}
	```
- etc!!

---

##### resources

- [TypeScript for JS Programmers](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
- [The TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
- [Docs](https://www.typescriptlang.org/docs/)