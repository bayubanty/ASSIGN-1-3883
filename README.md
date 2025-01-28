# ASSIGN-1-3883
# Program Name: MainTbm.py (use the name the program is saved as)
# Course: IT3883/Section XXX
# Student Name: Awoh, Bayo
# Assignment Number: Lab #1
# Due Date: 01/27/2025
# Purpose: it a text based menu system tha allowed to add, display and clear ?
# List Specific resources used to complete the assignment.

def text_based_menu():
    input_buffer = ""  # Initialize an empty input buffer

    while True:
        # Display the menu
        print("\nMenu:")
        print("1. Type in input")
        print("2. Clear the input ")
        print("3. Display the input ")
        print("4. Exit the program")

        # Get the user's choice
        choice = input("Enter your number (1-4): ").strip()

        if choice == "1":
            # Append data to the input buffer
            data = input("Enter a string to append: ")
            input_buffer += data
            print("Data added successfully!")

        elif choice == "2":
            # Clear the input buffer
            input_buffer = ""
            print("Input cleared.")

        elif choice == "3":
            # Display the input buffer
            if input_buffer:
                print("Current input:", input_buffer)
            else:
                print("Input  is empty.")

        elif choice == "4":
            # Exit the program
            print("Exiting program. Goodbye!")
            break

        else:
            # prompt for invalid choice
            print("Invalid choice. Please enter a number between 1 and 4.")

# Run the program
if __name__ == "__main__":
    text_based_menu()
