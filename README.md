import datetime

print("I-Rise : Hello! I am Your AI Chatbot I-Rise.")
print("What's your name?")
user_name = input("You: ")

print(f"I-Rise : Nice to meet you, {user_name}!")

while True:
    user_input = input(f"{user_name}: ").lower()

    if "hello" in user_input or "hi" in user_input:
        print("I-Rise : Hello there! How can I help you?")
    elif "how are you" in user_input:
        print("I-Rise : I'm great! What about you?")
    elif "who is your creator" in user_input:
        print(f"I-Rise : My creator is {user_name}")
    elif "i am fine" in user_input or "great" in user_input:
        print("I-Rise : Good Sir! How can I help you!?")
    elif "bye" in user_input or "exit" in user_input:
        print("I-Rise : Goodbye! Have a nice day.")
        break
    elif "your name" in user_input:
        print("I-Rise : I'm your AI ChatBot I-Rise.")
    elif "date" in user_input:
        today = datetime.datetime.now().strftime("%A, %d %B %Y")
        print(f"I-Rise : Today's date is {today}")
    elif "time" in user_input:
        current_time = datetime.datetime.now().strftime("%I:%M %p")
        print(f"I-Rise : Current time is {current_time}")
    else:
        print("I-Rise : Sorry, I didn't understand that.")
