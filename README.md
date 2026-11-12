# EXP 02 – React Lab Exercise: Using Props

## NAME: Monisha L

## REG NO: 2305001019

---

## Aim

To create a React application that demonstrates passing data from a parent component to a child component using props.

## Objectives

- To create a React project using Vite.
- To create a reusable Employee component.
- To pass employee details such as name, ID, department, and designation using props.
- To display multiple employees using the same component.
- To understand props destructuring and one-way data flow in React.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest props-demo -- --template react
cd props-demo
npm install
npm run dev
```

### Step 2: Create Employee.jsx

```jsx
function Employee({ name, id, department, designation }) {
  return (
    <div>
      <h2>Employee Details</h2>
      <p>Name: {name}</p>
      <p>ID: {id}</p>
      <p>Department: {department}</p>
      <p>Designation: {designation}</p>
      <hr />
    </div>
  );
}

export default Employee;
```

### Step 3: Write App.jsx

```jsx
import Employee from "./Employee";

function App() {
  return (
    <div>
      <h1>Employee Information</h1>

      <Employee
        name="Monisha"
        id="2305001019"
        department="CSE"
        designation="Software Developer"
      />

      <Employee
        name="user123"
        id="102"
        department="IT"
        designation="Web Developer"
      />

      <Employee
        name="user456"
        id="103"
        department="AIDS"
        designation="Data Analyst"
      />
    </div>
  );
}

export default App;
```

## Output

<img width="492" height="371" alt="image" src="https://github.com/user-attachments/assets/fcdf1099-549e-4c95-ba12-b5d6f5176ebc" />


## Result

Thus, a React application was successfully created and executed to demonstrate passing employee information from a parent component to a child component using props.
