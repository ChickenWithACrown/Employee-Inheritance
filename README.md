# JavaScript: Employee Inheritance

## Project Overview

This repository contains a JavaScript code solution for implementing prototypal inheritance in a scenario involving `Employee` and `Engineer` classes. The goal is to create a simple employee hierarchy using JavaScript's prototypal inheritance mechanism.

## Problem Statement

You need to implement a basic employee hierarchy where:

1. **Employee**:
   - Takes a `title` as input.
   - Has functions to `setTitle` and `getTitle`.

2. **Engineer (Inherits from Employee)**:
   - Takes `title` and `isManager` as input.
   - Inherits `setTitle` and `getTitle` from `Employee`.
   - Has additional functions to `setIsManager` and `getIsManager`.

## Code Structure

The project is organized into the following files:

- **`Employee.js`**: Contains the `Employee` class definition.
- **`Engineer.js`**: Contains the `Engineer` class definition.
- **`index.js`**: Contains the main function that handles input, object creation, and output.

## Usage

### How to Run the Code

1. Ensure you have [Node.js](https://nodejs.org/) installed.
2. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/employee-inheritance.git
   ```
3. Navigate to the project directory:
   ```bash
   cd employee-inheritance
   ```
4. Run the code:
   ```bash
   node index.js
   ```

### Input Format

The code reads input from the console in the following format:

- **Line 1**: A string (`title`) and a boolean (`isManager`) separated by space, representing the `Engineer` object properties.
- **Line 2**: A new string (`title`) to be set for the `Engineer` object.
- **Line 3**: A new boolean (`isManager`) to be set for the `Engineer` object.

### Example Input

```
SoftwareEngineer true
LeadEngineer
false
```

### Output Format

The program will print the following information:

1. **Initial Employee and Engineer Profile**:
   - The initial values of `title` and `isManager` for the `Engineer` object.
   
2. **Updated Engineer Profile**:
   - The updated `title` and `isManager` after using setter functions.
   
3. **Prototype Verification**:
   - Confirmation that the `Engineer` prototype has the expected properties (`setTitle`, `getTitle`, `setIsManager`, `getIsManager`).

### Example Output

```
Engineer object created with title: SoftwareEngineer and isManager: true
Title updated to: LeadEngineer
isManager updated to: false
Engineer object details - title: LeadEngineer, isManager: false
Engineer.prototype has property setTitle: true
Engineer.prototype has property getTitle: true
Engineer.prototype has property setIsManager: true
Engineer.prototype has property getIsManager: true
```

## Concepts Demonstrated

This project demonstrates key JavaScript concepts:

1. **Prototypal Inheritance**:
   - The `Engineer` class inherits from `Employee`, allowing the `Engineer` to use the `setTitle` and `getTitle` methods from the `Employee` prototype.

2. **Object Creation**:
   - An `Engineer` object is created with both `title` and `isManager` values.

3. **Property Access and Modification**:
   - Methods are used to set and get the `title` and `isManager` properties of the `Engineer` object.

4. **Prototype Verification**:
   - The code verifies if the `Engineer` prototype has the necessary methods (`setTitle`, `getTitle`, `setIsManager`, `getIsManager`) to ensure the inheritance was implemented correctly.

## License

This project is licensed under the MIT License.
