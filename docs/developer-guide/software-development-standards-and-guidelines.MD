## JAC DIGITAL
#### General Software Development Standards and Guidelines

- Version 1.0 February 2021

#### Revision History

 - Date Version Description 20/02/2021 1.0 -  Initial version

#### 1.  Introduction

The JAC Digital team develops and maintains software applications used in the process of candidate selection for judicial office in England and Wales and some tribunals with UK-wide powers.

These applications are becoming a critical component supporting the JAC operations and it is essential that they are well-written and maintained. Well-written software will contain fewer bugs and will run more efficiently. It will be easier for the current development team and future code keepers to maintain and modify the software as needed and this will lead to increased developer productivity and reduced costs of improving the existing codebase and development of new features.

It is important to note that the described standards and guidelines are not fixed and will evolve over time. Developers are encouraged to provide feedback to help to improve current ways of planning, writing and testing the applications.

#### 2.  Internal documentation standards

The current JAC applications are built using Javascript – Vue.js framework on the front-end, supported by Google Firestore database and various Google Cloud services. The Digital team has a repository where all existing documentation is kept - the JAC Documentation repository. We also use Miro boards and Zeplin to record design decisions.

#### 3.  General Javascript Guidelines

The JAC applications make use of the automatic code checking (linting), which simplifies following these guidelines. The lint plugin should be enabled in the IDE during development. You can also manually run the lint checker using command npm run lint. The application build will fail if linting rules are not respected.

Here are some examples of checks performed by lint:

We use the expanded syntax and spacing between operands, parameters etc. to maximize readability:

function weekendPlans (weather) { if (weather === ‘sunny’) { goToBeach(‘car’, [‘sunglasses’, ‘beach towel’]); } }

We use JS-style comments to document the code:

// This is a comment

We use common ES6 features – let/const, template literals, arrow functions etc.

We give preference to const over let if a variable not to be reassigned:

const myName = ‘Chris’; greetUser(‘Chris’);

We put ternary operators on a single line:

function getFee(isMember) { return (isMember ? '£2.00' : '£10.00'); }

We use strict equality and inequality:

myName === ‘Chris’; age !== 40;

We use template literals:

const myName = ‘Chris’; console.log(`Hi! I’m ${myName}!`);

For variable and function names we use lowerCamelCasing, and concise, human-readable, semantic names where appropriate:

const name = ‘Chris’; function greetUser (name) { // function notObviousName () { … } alert(`Hi! I’m ${name}!`); }

Some of the existing industry coding standards: MDN Webdocs AirBnB Javascript style guide Vue.js style guide

#### 4.  Coding Guidelines

General coding guidelines provide developers with a set of best practices which can be used to make applications easier to read and maintain.

A set of guidelines to follow:

Do not write or keep unused code.

Remove any console.log statements before pushing to the development branch.

Follow the DRY principle (Don’t Repeat Yourself). Extract duplicated code and place it in helper functions and reusable components into a shared repository (jac-kit).

Make use of constants instead of hard-coded values where it makes sense.

Familiarise yourself with the project architecture and ensure new components go into relevant folders.

Make sure names of components and names of files are the same, i.e.

Inside the component:

export default { name: ‘PackageManager’, … }

File name: PackageManager.vue, not Manager.vue or PackageEditor.vue and definitely not Abcdz.vue.

Do not write huge monolithic pieces of code that are difficult to read. Consider cyclomatic complexity of functions, split code into multiple, easy to understand components that do one job and do it well.

Write self-contained components that do not depend on code around them and can be easily reused.

Write code defensively. Do not follow only the correct path, always think of scenarios where something can go wrong, what will happen on invalid input, what might fail. This will help to catch many bugs before they happen.

Ask yourself how easy it would be to understand your coding decisions. If possible, document and/or provide diagrams to explain more complex features to colleagues.

#### 5.  Security

All sensitive data should be kept secure and accessed only by authorised personnel.

No hard coding of user ids’, names, passwords and sensitive data storage/access details. Please take care when commenting/creating bug tickets on Zen-hub and ensure you do not include any sensitive information, such as names or email addresses.

All data entered into the system by users has to be validated.

#### 6.  License/Terms of use/Legal requirements

Whilst planning new and reviewing existing application features, the licensing of any frameworks, packages, tools, graphics etc. created by other developers/organisations and used by the JAC should be investigated and their terms of use must be respected to avoid any legal issues.