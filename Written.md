<h1>CLASS 02(theory 1)</h1>
Difference between <em> and <i>
According to me, <em> is used to emphasise or for stressing a word and both <i> and <em> are both considered italic. Also, <em> tag is a semantic element, also <em> tag allows screen reader to be able to know that we are italizing a text for example <p>I love <em>cats</em> so much</p>. The word cats is emphasized or italic like the word "cats" is a little bit bend when i run that code. While the <i> tag is also used for italic but it's not semantic and they mostly used it before the use of html 5. So, <em> is the best tag to use compare to <i>.

<h1>Class 02(theory 2)</h1>
Certain elements were treated specially by the screen readers because they are semantic and they convey important structure and easy to read by users. The first element is the <img> element with alt attribute.The <img> element is treated specially because the screen reader will be able to read the alternative text incase if our image did not show. The alt attribute tells more about the image we are trying to convey to the screen readers.  The second element is the <a> element, it allows the screen readers to navigate through diffent links of a page by clicking on the text inbetween the opening and closing of <a>. The third element is the <button> element,it allows screen readers to know that we are dealing with clickable buttons.

<h1>CLASS 02 THEORY 03</h1>
Good use of aria-label
Icon-only button
Visually, the button is obvious because it shows a search icon. But a screen reader has no text to announce. for example;
<button aria-label="Search">
  🔍
</button>
Without the label, many screen readers would announce something unhelpful like:button but with aria-label, we have: Search, button.
This is exactly what aria-label is for: giving an accessible name to a control that otherwise has none.
Bad use: fixing non-semantic HTML with ARIA
Suppose someone creates a clickable element like this:
<div aria-label="Submit form">
  Submit
</div>. This is not a button because;
•	Not keyboard accessible by default
	•	Doesn’t respond to Enter/Space like a button
	•	Screen readers won’t treat it as a button
Adding an aria-label doesn’t solve any of those issues.
Fix the Html instead
<button type="submit">
  Submit
</button>
Now you get:
	•	Correct semantics
	•	Keyboard support
	•	Screen reader support
	•	Proper browser behavior

No ARIA needed.
)

<h1>CLASS ONE THEORY 2</h1>
What problems QUIC solves and why it matters for users in 2026?
QUIC allows our page to load faster for example when we are using apps that is connected to the server. QUIC enables us to change from unrelaible network connection to a more relaible one e.g from 4G to 5G. Also, Quic matters to users in 2026 because it helps video to stream very well on mobile app, fewer interruptions when moving between wifi and cellular and also, websites often start loading faster

<h1>CLASS ONE PRODUCT THINKING ONE</h1>
If i'm building a blog for a famous chef who wants more traffic; i'm going to use the <header> element first which will contain <h1> element.
The <header> will contains the article title, publication date, the name of the chef. The header element helps to identify the page title and it also helps us to understand what the content of the page is based on. The <main> will contains the primary content of the page and inside the main element is where i'm going to nest an article element.Each recipe or blog post are going to be wrapped in an <article> element, The <article> element helps the search engine identify individual posts that can rank differently. The <aside> element is like a side bar in our page,it contains related but non-essential information.It's also helps search engine to distinguish between supporting content from the main article.

<h1>CLASS ONE ENGINEERING BEST PRACTICE</h1>
I disagree using div everywhere in our html code because in terms of accessibility, screen readers rely on semantic html like the <header> <main> <nav> <article> and <footer> to understand the structure of a page and if everything is wrapped in a div, the screen readers won't be able to navigate the site efficiently. In terms of SEO, search engine often requires semantic html in order to analyze and understand our page structure efficiently. In terms of code maintainability, using semantic html allows other developers to understand our code much better, in contrast to large number of nested divs can make our code to be confusing and harder to maintain. Finally, while using only <div> elements may seem faster in the short term,semantic html creates websites that are more accessible, easier to maintain and better understood by search engines.

<h1>CLASS ONE THEORY 1</h1>
Structure of the DOM TREE
  html
 ---head
  ---meta
  ---title
 ---body
  ---header
   ---nav
   ---h1
  ---main
   ---article
    ---section
   ---aside
  ---footer
  understanding the DOM trees for a web developer helps us to represent the structure of a webpage in a way that javascript can read and change the content, structure and style and it also helps to improve our debugging skills.
  
  <h1>CLASS 03 THEORY 01</h1>
If a designer hands me a 5 MB PNG hero image, I wouldn’t just compress it and upload it. I’d treat it as a performance optimization task and work through a pipeline.
Step 1: Determine Whether PNG Is Even Appropriate
Step 2: Check Actual Display Size
Step 3: Convert to Modern Formats
Step 4: Compress Intelligently
Step 5: Generate Responsive Variants
Step 6: Use a CDN
Step 7: Prioritize the Hero Image
Step 8: Lazy Load Everything Else
Step 9: Verify Core Web Vitals
Step 10: Automate the Pipeline.}
  
 <h1>CLASS 03 THEORY 02</h1>
  The srcset attribute is used on an <img> element to provide multiple versions of the same image at different sizes. when we use an srcset attribute on an image, the browser automatically chooses the most appropriate image based on user's device and screen size.
  A scenario whereby a user wants to display a product image on a website e.g 
  <img src="product-400.jpg" srcset="product-400.jpg 400w
          product-800.jpg 800w
          product-2000.jpg 2000w"
  sizes="100vw" alt="running shoes">
  A phone with a 360px screen downloads product-400.jpg
  A tablet may download product-800.jpg
  A large desktop monitor may download product-2000.jpg.
  
  <h1>CLASS 03 THEORY 03</h1>
  rel="noopener" is important when using target="blank" because it prevents a new tab to interact with the original tab. it creates a safety barrier between the two tabs. Without the noopener, the new page can change our original page's location, also when using a banking website it can easily redirects the user to a fake login page that looks legitimate.
  For a non-technical person,think of your browser tabs as your phone and noopener as a pin
  without noopener;A person can access your phone and steals improtant information on it like your banking app and  easily transacts money from your account
  With noopener; A person won't be able to access your phone because it will require a pin .
  
<h1>CLASS 05 THEORY 0NE</h1>
If two adjacent divs have margin-bottom : 20px and margin-top: 30px, Tge space inbetween them is 30px. The reason is because CSS uses margin collapsing for adjacent vertical margins, so the browser uses the largest margin value. Also, CSS use margin collapsing because it helps to avoid unnecessary space between adjacent margins. so, the space in between the two divs is 30px.

<h1>CLASS 05 THEORY TWO</h1>
Css specificity determines which rule is applied when multiple selectors target the same element. How to calculate the specificity of wach selector;
1. .header nav ul li a: .header-1 class = 0,0,1,0; nav ul li a- 4 elements = 0,0,0,4. Total: 0,0,1,4
2. nav a.active: .active- 1 class = 0,0,1,0; nav,a: 2 elements = 0,0,0,2. Total: 0,0,1,2
3. .nav-links a: .nav-links: 1 class = 0,0,1,0; a: 1 element = 0,0,0,1. Total: 0,0,1,1.
.header nav ul li a wins because its specificity (0,0,1,4) is higher than (0,0,1,2) and (0,0,1,1){()}

<h1>CLASS 05 THEORY 03</h1>
Cascade is the  set of rules the browser uses to decide which which css declaration get applied when multiple rules targetthe same element. For example; i'm stying a button in a header element, the existing css is;
button {
 background-color: blue; 
} and if the designer wants the button in the header to be green then i can give it a class name of button-1. so, my new css will be 
.button-1{
 background-color: green;
}
so, the new style will override the previous one.

<h1>CLASS 05 ENGINEERING THINKING ONE</h1>
if i use padding: 10px; and it becomes wider, that is because the default for box-sizing is content box and using content box only makes the width to be applied to the content area alone. For example, .card {
           width: 200px;
           padding: 10px;
} the element content area becomes wider with the padding added but with border-box; the browser includes padding and borders within the declared width. The element remains exactly 200px wide by making the content area width to be 180px, 10px left padding and 10px right padding.

<h1>CLASS 05 ENGINEERING THINKING TWO</h1>
The content-box only makes our width or height of an element to be become wider or longer. for example,
div {
 width: 320px;
 padding: 10px;
 border: 5px solid black;
} if i want to calculate the width of this element for content box then i will have 320 + 10 + 10 + 5 + 5 making it 350px. This means that the content area becomes more wider. 
The border-box allows the calculation of the padding and border from the given width. This makes our content area to be smaller compare to when we use content-box. for example
div {
 width: 300px;
 padding: 10px;
 border: 5px solid black;
}. here, the content area width is 270px, right padding 10px, left padding 10px, right border 5px and  left border 5px which make the element exactly 300px wide.

<h1>CLASS O6 THEORY 01</h1>
Flex-grow property specifies how much an item will grow relative to the rest of the flexible items inside the same container.
The flex-basis property specifies the intial length of a flexible item.
Flex-shrink property specifies how the item will shrink relative to the rest of the flexible items inside the same container.

<h1>CLASS O6 THEORY 02</h1>
Align item: stretch; will not work if the items already has a fixed width and height. For example
<div class="container">
  <div class="item">Box 1</div>
  <div class="item">Box 2</div>
  </div>
  .container {
    display: flex;
    align-items: stretch;
    height: 300px;
  }
  .item {
    height: 100px;
    width: 100px;
  }
  For the stretch property, the three boxes suppose to stretch to fill the container's 300px but it won't stretch because each items already has an explicit height. so, the height of the three boxes will remain 100px.
  
  <h1>CLASS 06 ENGINEERING THINKING TWO</h2>
  In my project, the flexbox ensures that logo is positioned at the end, my navigation items is at the middle and my harmburger stays right. Instead of building two menus, i show .nav on desktop, hide it on mobile and replace it with a harmburger toggle.

<h1>CLASS 07 THEORY one</h1>
CSS-grid is used for two-dimensional layout, with rows and colums while CSS flex box is used for one-dimensional layout, with rows or columns. We choose grid when we need control over rows and columns simultaneously for example dashboarbs, galleries, and page layouts. We choose flex when we need to lay out items in a single row or columns for example navbars, button groups.

<h1>CLASS 07 THEORY 02</h1>
grid-template-areas is a CSS Grid feature that lets you name sections of your layout visually, then place elements into those named regions.
Instead of thinking in numbers (columns/rows), you think in layout “shapes”.
Basic Example:
<div class="layout">
  <header class="header">Header</header>
  <aside class="sidebar">Sidebar</aside>
  <main class="content">Main</main>
  <footer class="footer">Footer</footer>
</div>

.layout {
  display: grid;

  grid-template-columns: 200px 1fr;
  grid-template-rows: auto 1fr auto;

  grid-template-areas:
    "header  header"
    "sidebar content"
    "footer  footer";

  height: 100vh;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.content { grid-area: content; }
.footer { grid-area: footer; }
How to read it:
This part;
grid-template-areas:
  "header  header"
  "sidebar content"
  "footer  footer";
  is literally a visual map of the page.
When grid-template-areas makes sense
1.When you are building a full page layouts like dashboard, blogs etc
2. When you want a responsive rearrangement
3. when fellow developers need readable layout code 


<h1>CLASS 08 THEORY ONE</h1>
The utility-first philosophy is the idea that you build UI by composing many small,single-purpose CSS classes directly to your html, rather than creating custom semantic classes and writing CSS for each component.
The tailwind creator prefers utility classes because it reduces the css growth,avoid naming things,makes changes faster,encourages consistency and prevents dead css.

<h1>CLASS 08 THEORY TWO</h1>
The JIT compiler is a Tailwind's engine that generates CSS only for the utility classes one actually use instead of generating the entire tailwind framework upfront.
How it affects Css file size;
without optimization, a tailwind build can be several megabytes because it contains thousands of utilities and variants. JIT only generates classes flund in your source file, so the production bundle contaons little or no unused Css. As a result,production Css oftens ends up in the tens of kilobytes rather than megabytes, depending on how many utilities your application actually uses.

<h1>CLASS 08 PRODUCT THINKING</h1>
1. Readability:readability in real projects isn’t about how clean a single line looks—it’s about how quickly you can understand what a component does without jumping between files.
With Tailwind:
	•	All styles are visible in place
	•	No need to search styles.css, navbar.css, card.scss, etc.
	•	You immediately see layout, spacing, color, and behavior together
2. Maintainability: 
Maintainability problems usually come from:
	•	duplicated CSS rules across files
	•	inconsistent spacing/colors
	•	unclear naming conventions (.card, .card2, .card-new-final)

Tailwind solves this by enforcing:
	•	a single design system (spacing scale, colors, typography)
	•	no arbitrary CSS drift
	•	no hidden side effects in unrelated files
	3. Consistency: Actually, Tailwind improves consistency by design. fir example;
In Tailwind:
	•	spacing is constrained (mt-4, mt-5, etc.)
	•	colors are predefined (blue-500, gray-200)
	•	typography scales are standardized
 4. Performance: This is actually where tailwind is strongest
CSS performance:

Tailwind uses PurgeCSS / content-based tree-shaking:
	•	unused styles are removed in production
	•	final CSS is usually very small
	
<h1>CLASS 08 ENGINEERING THINKING ONE</h1>
What this project demonstrates
1. Base Card system
All cards uses:rounded-xl border bg-white p-5 transition and this creates a UI foundation.
2. Hover interaction:hover:-translate-y-1 hover:shadow-lg gives slight lift and stronger shadow.
3. Featured card uses:border-2 border-blue-500 scale-105 shadow-md
meaning: thicker border, scale and stronger color 
4. Responsive grid layout system:grid grid-cols-1 md:grid-cols-3 gap-6
this means 1 column on mobile; 3 colums on desktop and clean spacing system.

<h1>CLASS 09 THEORY 01</h1>
Tailwind’s Breakpoint System
Tailwind uses a mobile-first responsive design approach.

That means:
	1.	Classes without a breakpoint apply to all screen sizes.
	2.	Breakpoint-prefixed classes apply at a specific screen width and larger.
How md: Works
Suppose you write:
<div class="bg-blue-500 md:bg-red-500">
  Card
</div>
Tailwind generates CSS similar to:
.bg-blue-500 {
  background: blue;
}

@media (min-width: 768px) {
  .md\:bg-red-500 {
    background: red;
  }
}
Result:
Phone (500px)     → Blue
Tablet (800px)    → Red
Desktop (1400px)  → Red
Because md: means: Apply this style at 768px and above.
Creating a Custom 1200px Breakpoint
In a tailwind configuration file:
// tailwind.config.js

module.exports = {
  theme: {
    extend: {
      screens: {
        desktop: '1200px',
      },
    },
  },
};
now you can use: 
<div class="
  text-sm
  desktop:text-xl
">
  Example
</div>
meaning:
<1200px   → text-sm
≥1200px   → text-xl

<h1>CLASS 09 THOERY 02</h1>
Arbitrary values let you write custom CSS values directly inside class names using square brackets.
Example: <div class="w-[123px] h-[37px] bg-[#1a1a1a]">
Instead of being limited to Tailwind’s predefined scale (w-1, w-2, w-64, etc.), you can define exact values inline.
How they work:
 Tailwind converts :w-[123px] into width: 123px;
So it’s basically a way to write on-demand CSS inside your class string.
When arbitrary values are useful
1. One-off design tweaks
2. Rapid prototyping. 
3. Dynamic or computed values
When to extend the Tailwind config instead: use tailwind.config.js when:
1. The value is reused across the system
2. You want semantic meaning
3. You want design consistency
4. You want better maintainability

<h1>CLASS 10 THEORY 01</h1>
1. Scope
var is function-scoped; for example
function test() {
  if (true) {
    var x = 10;
  }
  console.log(x); // 10
} it ignores block scope (if, for) and only respects function scope
let and const  are block-scoped; for example
 
function test() {
  if (true) {
    let a = 10;
    const b = 20;
  }
  console.log(a); // ReferenceError
  console.log(b); // ReferenceError
}
2. Hoisting
var is hoisted  and initialized as undefined
let and const are hoisted but not initialized
3. Reassignment
var can be reassigned and redeclared
let can be reassigned but not redeclared
const can neither be reassigned nor redeclared.
Why const does NOT make objects/arrays immutable
Example with object: 
const user = {
  name: "Alice"
};

user.name = "Bob"; // allowed
console.log(user); // { name: "Bob" }
Why does this work? Because const prevents:user = {} but not user.name = "Bob"
Example with arrays:
const numbers = [1, 2, 3];

numbers.push(4); // allowed
numbers[0] = 99; // allowed

numbers = []; // ❌ not allowed

<h1>CLASS 10 THEORY 02</h1>
The Temporal Dead Zone (TDZ) is the period of time between:when a variable is hoisted and when it is actually initialized.During this period, accessing the variable causes a ReferenceError and it applies to let and const.
It exists to prevent a dangerous class of bugs that were common with var.
Example where TDZ prevents a real bug
for example;
function initApp() {
  console.log(config.apiUrl);

  let config = {
    apiUrl: "https://api.example.com"
  };
}

initApp();
now you get:ReferenceError: Cannot access 'config' before initialization
Why this is better
	•	You immediately know something is wrong
	•	You don’t continue execution with bad data
	•	The bug is easier to debug

<h1>CLASS 10 PRODUCT THINKING</h1>
For a calculator app, the choice between const and let comes down to one key idea:

Use const when the variable should not be reassigned to a new value. Use let when the value must change during user interaction.A calculator is stateful (it evolves as the user clicks buttons), so most values will actually be let.

Let’s break it down properly.
1. Display value → let
why let?
Because the display changes constantly:
	•	user types 5 → "5"
	•	user presses + → "5+"
	•	user types 3 → "5+3"
	•	result → "8"

So you are continuously reassigning the value.
2. Operator → let
why let?
The operator changes as the user interacts: + - * /
3. Previous operand → let
 why let?
This value updates during calculation cycles:
User input:  12 + 7
Step 1 → previousOperand = 12
Step 2 → operator = "+"
Step 3 → currentOperand = 7
Step 4 → result = 19
Step 5 → previousOperand = 19 (for next operation)
so, it continously changes.
4. So do we use ANY const?

Yes—but for things that don’t change reference.
Example: DOM elements → const 
const display = document.querySelector(".display");
const buttons = document.querySelectorAll(".btn");
why const?
Because:
	•	You are not reassigning the variables
	•	The element references stay the same

You might change the content, but not the variable itself:
display.textContent = "123"; // allowed
but not: 
display = document.querySelector(".other"); // ❌ not allowed


<h1>CLASS 11 THEORY ONE</h1>
In JavaScript, == and === are both comparison operators, but they behave very differently.
1. === (Strict Equality)
	•	Compares value + type
	•	No type conversion happens
for example:5 === 5        // true
5 === "5"      // false
0 === false    // false
null === undefined // false
2. == (Loose Equality)
	•	Compares values after type coercion
	•	JavaScript tries to convert both sides to the same type first
for example:5 == "5"       // true
0 == false     // true
"" == false    // true
null == undefined // true
3. Why == can cause bugs

Because JavaScript performs implicit type conversion, results can be surprising.
Real Bug Example: Form Validation
Imagine checking if a user entered a valuefunction isEmpty(value) {
  return value == 0;
}
now test:isEmpty("")      // true ❌ unexpected
isEmpty(false)   // true ❌ unexpected
isEmpty("0")     // true ❌ unexpected
Why this happens
JavaScript coerces values:""   → 0
false → 0
"0"  → 0
So everything becomes 0, and the check incorrectly passes.
Correct Version (===)
function isEmpty(value) {
  return value === 0;
}
now:isEmpty("")     // false
isEmpty(false)  // false
isEmpty("0")    // false
isEmpty(0)      // true
much safer and predictable.

<h1>CLASS 11 THEORY TWO</h1>
Optional chaining is a JavaScript operator that lets you safely access deeply nested properties without throwing an error if something is null or undefined.Instead of crashing, it returns undefined.
1. Example: Nested object access (prevents crash): for example,
With optional chaining,
const user = {};
console.log(user?.profile?.name);
Output: undefined
2. Example: API response safety
Imagine an API that sometimes omits fields, with optional chaining;
const response = {
  data: null
}
console.log(response?.data?.user?.id);
returns undefined instead of theowing.
3. Example: Optional function calls
sometimes a callback may not exist for example:
const config = {};
with optional chaining,config.onSuccess?.();
safe no-op if function doesn't exist.
When optional chaining hides a bug ⚠️
for example;
function getUserName(user) {
  return user?.name;
} now call it incorrectly;getUserName(); // forgot to pass user
Output: undefined
Why this is dangerous

You expected a user object, but:
	•	No error is thrown
	•	Bug silently fails
	•	Problem may propagate downstream
	
	<h1>CLASS 11 THEORY 03</h1>
The nullish coalescing operator returns the right-hand value only when the left-hand value is null or undefined. for example;
const result = value ?? defaultValue;
meaning;
if (value === null || value === undefined) {
  result = defaultValue;
} else {
  result = value;
}
How is it different from ||?
The logical OR operator (||) returns the right-hand value when the left-hand value is falsy.
Falsy values in JavaScript include:
false
0
-0
0n
""
null
undefined
NaN
Example;const value = 0;

console.log(value || 10); // 10
Because 0 is falsy, || treats it as if no value was provided.
Example where ?? is correct and || fails
Imagine a website allows users to set the number of items shown per page,
function getItemsPerPage(userSetting) {
  return userSetting ?? 20;
}; if a user explicitly chooses;
const itemsPerPage = 0;
and you use ||: const result = itemsPerPage || 20;
console.log(result);
output: 20
This is wrong because the user intentionally chose 0.
Using ??:
const result = itemsPerPage ?? 20;
console.log(result);
output: 0
This is correct because 0 is a valid value and should not be replaced.

<h1>CLASS 12 THEORY ONE</h1>
In JS, the key difference between a function declaration and a function expression is how and when and the fuction is created and assigned.
A fuction declaration looks like this:
function greet() {
  console.log("Hello");
}
A function expression is when a function is created as part of an expression, usually assigned to a variable:
const greet = function() {
  console.log("Hello");
}
Why Hoisting behaves differently;
Function declaration are hoisted with their entire definition. That means javascript moves the function into memory before any code runs. for example;
greet();
function greet() {
  console.log("hello");
} even though greet() is called before it appears in the code,the engine already knows the full function. With function expressions, only the variable is hoisted not the function assignment.

<h1>CLASS 12 THEORY TWO</h1>
A pure function is a function that follows two rules:
1. Given the same arguments, it always returns the same result;
2. No side effects: it does not change anything outside itself.
Example of a pure function is;
function add(a,b) {
  return a + b;
} this means if you call add(2, 3), it will always return 5 and it doesn't modify anything outside itself and it only depends on its inputs.
Developers value pure functions because it is predictable, easier to test,easier to debug, safer in large applicationsand great for functional programming.

<h1>CLASS 12 THEORY 03</h1>
A callback is a function that we pass into another function so it can be used later. Higher- order function is any  function that takes another function as an argument or returns a function. Callbacks and higher-order functions are fundamental to javascript because;
1. Asynchronous programmingdepends on callbacks
2. They power arrays methods
3. They make codes reusable

<h1>CLASS 12 PRODUCT THINKING</h1>
if i'm building a math utility library for a calculator app, pure functions are exactly what i want everywhere. Here are 6 examples of pure fuctions each with what they do, inputs, outputs
1. add(a,b)
. adds two numbers
Inputs: a(number), b(number)
Outputs: sum of a + b
for example;
function add(a, b) {
  return a + b;
}
add(2,3); // 5
2. substract(a,b)
for example;
fuction substract(a,b) {
  return a - b;
}
substract(10, 4) // 6
3. multiply(a,b)
for example;
function mumtiply(a,b) {
  return a * b;
}
multiply(6, 7) // 42
4. divide(a,b)
for example;
function divide(a,b) {
  return a / b;
}
divide(20, 5) // 4
5. power(base, exponent)
for example;
function power(base, exponent) {
  return base ** exponent;
}
power(2, 3) // 8
Why making these functions pure makes my code better is;
1. predictable calculations
2. reusability across the app

<h1>CLASS 12 ENGINEERING THINKING ONE</h1>
A compose function is a higher-order function that takes multiple functions and combines them into a single function, where each function is applied right-to-left. So,compose(f, g, h)(x) = f(g(h(x)))
1. Simple Implementation (using a loop)
function compose(...fns) {
  return function (x) {
    let result = x;

    // apply from right to left
    for (let i = fns.length - 1; i >= 0; i--) {
      result = fns[i](result);
    }

    return result;
  };
}
How it works: Given;
const add1 = x => x + 1;
const double = x => x * 2;
const square = x => x * x;

const fn = compose(add1, double, square);
calling;fn(3)
execution flow:square(3) → 9
double(9) → 18
add1(18) → 19
so, result = 19
2. Same Implementation Using reduce

We can replace the loop with reduceRight, which naturally processes right-to-left for example;
function compose(...fns) {
  return function (x) {
    return fns.reduceRight((acc, fn) => fn(acc), x);
  };
}
Why reduceRight works better here
	•	reduce() processes left → right
	•	reduceRight() processes right → left (perfect for composition)
Step-by-step with reduceRight
fns = [f, g, h]
x = input
Execution: acc = x
→ h(x)
→ g(h(x))
→ f(g(h(x)))

<h1>CLASS 13 THEORY ONE</h1>
When to choose an array:
use an array when;
. Order matters
. You're working with a lists of items
. You meed to loop through everything
. You care about positions (index 0,1,2,...)
When to choose an object:
use an object when;
. You want to label or describe values
. You need fast lookup by name(key)
. The structure represents a real world entity
Real example where an object is clearly better;
const user = {
  name: "John",
  age: 25,
  city: "lagos",
  isActive: true
};
why the object is clearly better here;
1. Self-documenting: you immediately understand the name, age and city
2. Safer access
3.easy update without breaking structure: you can add new field safely for example user.email = "john@email.com"
4. Better for real-world entities: objects naturally model things like; users, products, settings, API reponses.

<h1>CLASS 13 THEORY 02</h1>
Destructuring lets you "unpack" values from objects into variables. with nested objects, you can reach deep properties in a single, clean statement.For example,
const {
  data: {
    user: {
      name,
      contact: {
        email,
        address: { city }
      }
    }
  }
} = response

<h1>CLASS 14 THEORY ONE</h1>
Event bubbling and event capturing are two phases of how events propagate through the Document Object Model) when a user interacts with an element.
Event Propagation Phases is when an event occurs (e.g a button click) it traves through three phases:
	1.	Capturing phase (top → down)
	2.	Target phase (the element that triggered the event)
	3.	Bubbling phase (bottom → up)
For example, given:
<div id="parent">
  <button id="child">Click Me</button>
</div>; the event path is:
document
  ↓
html
  ↓
body
  ↓
parent
  ↓
child  (target)
  ↑
parent
  ↑
body
  ↑
html
  ↑
document
Event Capturing
In the capturing phase, the event moves from the outermost ancestor down toward the target element.
parent.addEventListener("click", () => {
  console.log("Parent (capturing)");
}, true); // true enables capturing

child.addEventListener("click", () => {
  console.log("Child");
}); output when the button is clicked:
Parent (capturing)
Child
The parent handler runs before the event reaches the child.
Event Bubbling
In the bubbling phase, the event moves from the target element back up through its ancestors.for example;
parent.addEventListener("click", () => {
  console.log("Parent (bubbling)");
});

child.addEventListener("click", () => {
  console.log("Child");
}); the output is ;
Child
Parent (bubbling).This is the default behavior for most event listeners.
When to Choose Event Bubbling
Event bubbling is the most common choice because it supports event delegation efficiently.for example;
document.getElementById("parent").addEventListener("click", (e) => {
  if (e.target.tagName === "BUTTON") {
    console.log("A button was clicked");
  }
});
Instead of attaching listeners to many buttons, one listener on the parent can handle them all.
Use bubbling when:
	•	Implementing event delegation.
	•	Handling events from dynamically added elements.
	•	Following standard DOM behavior.
When to Choose Event Capturing
Use capturing when you need to intercept an event before it reaches the target.
Example use cases:
	•	Global logging or analytics.
	•	Security or validation checks before child handlers run.
	•	Frameworks or libraries that need early access to events.
	•	Preventing certain interactions before target elements process them.
document.addEventListener("click", (e) => {
  console.log("Captured before target");
}, true);

<h1>CLASS 14 THEORY 02</h1>
Event delegation is a technique where you attach a single event listener to a parent element and use event bubbling to handle events from its child elements.
Instead of adding a listener to every child, you add one listener to a common ancestor and determine which child triggered the event using event.target.
With Event Delegation
Attach a single listener to the parent:
const menu = document.getElementById("menu");

menu.addEventListener("click", (event) => {
  if (event.target.tagName === "BUTTON") {
    console.log(event.target.textContent);
  }
});
Now:
	•	Only one listener exists.
	•	All current buttons work.
	•	Future buttons work automatically.
	•	Less code and better performance for large collections.
Scenario: Dynamic Todo List

Imagine a todo application where users can add tasks at any time.
With event delegation;
const todoList = document.getElementById("todoList");

todoList.addEventListener("click", (event) => {
  if (event.target.classList.contains("delete")) {
    event.target.parentElement.remove();
  }
});
Now every delete button works:
	•	Existing tasks 
	•	Newly added tasks 
	•	Removed tasks require no cleanup 
	
	<h1>CLASS 14 THEORY 03</h1>
The main security concern is Cross-Site Scripting (XSS).

When you use innerHTML, the browser treats the string as HTML and parses it. If that string contains malicious code supplied by a user or an untrusted source, an attacker may inject scripts or harmful markup into your page.
Risk with innerHTML
const userInput = '<img src="x" onerror="alert(`Hacked`)">';

document.getElementById("output").innerHTML = userInput;
The browser creates the <img> element and executes the onerror handler when the image fails to load.
An attacker could potentially inject:
<img src="x" onerror="stealCookies()">
or other malicious content.
This is a classic XSS vulnerability.
Safer Approach: createElement + textContent
const userInput = '<img src="x" onerror="alert(`Hacked`)">';

const p = document.createElement("p");
p.textContent = userInput;

document.getElementById("output").appendChild(p);
The page displays:
<img src="x" onerror="alert(`Hacked`)">
as plain text instead of interpreting it as HTML.Because textContent does not parse HTML, the injected code cannot execute.

<h1>CLASS 14 PRODUCT THINKING ONE</h1>
For a real-time collaborative todo app, think of two separate problems:
	1.	Keeping every user’s DOM in sync
	2.	Resolving conflicts when users edit the same item
1. DOM Updates for Real-Time Collaboration
Assume updates arrive from a server via WebSockets.
A. New Todo Created
User A adds:
{
  "type": "todo_created",
  "id": 42,
  "text": "Buy milk"
}. All connected clients should:
const li = document.createElement("li");
li.dataset.id = 42;
li.textContent = "Buy milk";

todoList.appendChild(li);
Dom change:<li data-id="42">Buy milk</li>
B. Todo Edited
User A changes:Buy milk toBuy milk and eggs
Server broadcasts:{
  "type": "todo_updated",
  "id": 42,
  "text": "Buy milk and eggs"
}
clients update:const item = document.querySelector('[data-id="42"]');
item.textContent = "Buy milk and eggs";
C. Todo Completed
Broadcast:{
  "type": "todo_completed",
  "id": 42,
  "completed": true
}
Dom update:item.classList.add("completed");
D. Todo Deleted
Broadcast{
  "type": "todo_deleted",
  "id": 42
}
Dom update: document
  .querySelector('[data-id="42"]')
  ?.remove();:
All users instantly see the removal.
2. Handling Conflicting edits
Option 1: Last Write Wins (Simple)
Option 2: Delete Wins (Common for Todo Apps)
Option 3: Optimistic Locking / Version Numbers
Option 4: Operational Transform (OT) or CRDTs


