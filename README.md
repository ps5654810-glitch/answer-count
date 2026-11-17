def main():
    items = []
    while True:
        print("\n=== MY PYTHON CONSOLE APP ===")
        print("1. Add an item")
        print("2. View all items")
        print("3. Exit")
        
        choice = input("Choose an option (1-3): ")
        
        if choice == "1":
            name = input("Enter item name: ")
            items.append(name)
            print(f"Added '{name}'!")
        elif choice == "2":
            print("\nYour List:", items if items else "No items yet.")
        elif choice == "3":
            print("Closing app. Goodbye!")
            break
        else:
            print("Invalid choice. Please type 1, 2, or 3.")

main()
