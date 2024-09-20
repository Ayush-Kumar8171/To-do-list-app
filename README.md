DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Todo List app</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div class="wrapper show-category">
        <div class="screen-backdrop"></div>
        <div class="screen home-screen">
            <div class="head-wrapper">
                <div class="menu-btn">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25H12" />
                    </svg>
                </div>
                <div class="welcome">
                    <div class="content">
                        <h1>Hello Ayush</h1>
                        <p>Today you have <span class="totalTasks">5</span> tasks</p>
                    </div>
                    <div class="img">
                        <div class="backdrop"></div>
                        <img src="image/boy.png" alt="" srcset="">
                    </div>
                </div>
            </div>
            <!-- Categories -->
            <div class="categories-wrapper">
                <div class="categories">
                    <div class="category">
                        <div class="left">
                            <img src="image/boy.png" alt="" srcset="">
                            <div class="content">
                                <h1>Personal</h1>
                                <p>5 Tasks</p>
                            </div>
                        </div>
                        <div class="options">
                            <div class="toggle-btn">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 6.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 12.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 18.75a.75.75 0 110-1.5.75.75 0 010 1.5z" />
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Tasks Screen -->
        <div class="screen category-screen">
            <div class="head-wrapper">
                <div class="back-btn">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M6.75 15.75L3 12m0 0l3.75-3.75M3 12h18" />
                    </svg>
                </div>
                <div class="options">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M12 6.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 12.75a.75.75 0 110-1.5.75.75 0 010 1.5zM12 18.75a.75.75 0 110-1.5.75.75 0 010 1.5z" />
                    </svg>
                </div>
            </div>
            <div class="category-details">
                <img src="image/boy.png" alt="" srcset="" id="category-img">
                <div class="details">
                    <p class="category-tasks">8 Tasks</p>
                    <h1 class="category-title">Personal</h1>
                </div>
            </div>
            <div class="tasks-wrapper">
                <div class="tasks">
                    <div class="task-wrapper">
                        <label for="task" class="task">
                            <input type="checkbox" name="" id="task">
                            <span class="checkmark">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                                    <path stroke-linecap="round" strokeline-join="round" d="M4.5 12.75l6 6 9-13.5" />
                                </svg>
                            </span>
                            <p>Buy a new car</p>
                        </label>
                        <div class="delete">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                                stroke="currentColor" class="w-6 h-6">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                            </svg>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- add Task button -->
        <div class="add-task-btn">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M12 4.5v15m7.5-7.5h-15" />
            </svg>
        </div>

        <!-- backdrop -->
         <div class="black-backdrop"></div>
        <!-- add task form -->
         <div class="add-task">
            <div class="add-task-backdrop"></div>
            <h1 class="heading">Add Task</h1>
            <div class="input-group">
                <label for="task-input">Task</label>
                <input type="text" id="task-input" required>
            </div>
            <div class="input-group">
                <label for="category-select">category</label>
                <select name="" id="category-select"></select>
            </div>
            <div class="btns">
                <button class="cancel-btn">Cancel</button>
                <button class="add-btn">Add</button>
            </div>
         </div>
    </div>

    <script src="script.js"></script>
    <!-- font-family: "Inter", sans-serif; -->
</body>

</html>
