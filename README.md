# mini.adventure.game.py
def start_game():
    print("-------Welcome to Adventure Game-------")
    print("Tum ek jungle me ho...\n")

    choice1 = input("Left jao ya Right? (left/right): ").lower()

    if choice1 == "left":
        left_path()
    elif choice1 == "right":
        right_path()
    else:
        print(" Invalid choice! Game over")

def left_path():
    print("\n Tum left gaye aur ek river mili")

    choice = input("Tair kar cross karo ya bridge use karo? (swim/bridge): ").lower()

    if choice == "swim":
        print(" Koi crocodile ne attack kar diya! Game Over")
    elif choice == "bridge":
        print("CONGRATULATION")
        print(" Tum safely cross kar gaye aur Khazana mil gaya ")
    else:
        print(" Invalid choice!!!")

def right_path():
    print("\n Tum right gaye aur ek cave mili")

    choice = input("Cave me jao ya wapas jao? (enter/leave): ").lower()

    if choice == "enter":
        print(" Dragon mila... aur tum haar gaye! Game Over")
    elif choice == "leave":
        print(" Tum safe ho gaye. Game finished!!!")
    else:
        print("---Invalid choice!---")

if __name__ == "__main__":
    start_game()
