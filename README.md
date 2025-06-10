# Tasklist-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <h1>Todo Application </h1>
    <div>
        <!-- input and add button  -->
         <div>
            <input type="text">
            <button>add</button>
         </div>
         <!-- display tasks -->
         <div>
            <ul>
                <li>task 1 </li>
                <li>task 2 </li>
                <li>task 3 </li>
                <li>task 4 </li>
            </ul>
         </div>
    </div>
    
    <script src="./app.js"></script>
</body>
</html>
const addTodo = document.getElementById("addTodo")
const Tasklist = document.getElementById("tasklist") // ul tag get 


addTodo.addEventListener("click",function todo() {
    
    const inputtask = document.getElementById("inputtodo")

    // create one new li tag element 
    const newTodo = document.createElement("li")  
    
    newTodo.innerText = inputtask.value

    Tasklist.appendChild(newTodo)
    
})
