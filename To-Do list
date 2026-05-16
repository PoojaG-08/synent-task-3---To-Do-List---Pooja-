# Simple To-Do List Application

tasks = []

while True:
    print("\n===== TO-DO LIST MENU =====")
    print("1. Add Task")
    print("2. Delete Task")
    print("3. View Tasks")
    print("4. Exit")

    choice = input("Enter your choice: ")

    # Add Task
    if choice == "1":
        task = input("Enter task: ")
        tasks.append(task)
        print("Task added successfully.")

    # Delete Task
    elif choice == "2":
        if len(tasks) == 0:
            print("No tasks available.")
        else:
            print("\nTasks:")
            for i, task in enumerate(tasks, start=1):
                print(f"{i}. {task}")

            try:
                task_num = int(input("Enter task number to delete: "))

                if 1 <= task_num <= len(tasks):
                    removed = tasks.pop(task_num - 1)
                    print(f"Task '{removed}' deleted successfully.")
                else:
                    print("Invalid task number.")

            except ValueError:
                print("Please enter a valid number.")

    # View Tasks
    elif choice == "3":
        if len(tasks) == 0:
            print("No tasks in the list.")
        else:
            print("\n===== YOUR TASKS =====")
            for i, task in enumerate(tasks, start=1):
                print(f"{i}. {task}")

    # Exit Program
    elif choice == "4":
        print("Exiting To-Do List App...")
        break

    # Invalid Choice
    else:
        print("Invalid choice. Please select from the menu.")