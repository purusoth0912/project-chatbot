# project-chatbot
#chatbot 

# Simple rule-based chatbot without libraries

def chatbot():
    print("Chatbot: Hello! I'm a simple chatbot. Type 'bye' to exit.")

    while True:
        user_input = input("You: ").lower()

        if user_input in ["hi", "hello", "hey"]:
            print("Chatbot: Hello there! How can I help you?")

        elif user_input in ["how are you?", "how are you", "how's it going"]:
            print("Chatbot: I'm just a program, but I'm functioning as expected!")

        elif "your name" in user_input:
            print("Chatbot: I'm Chatbot AI. Nice to meet you!")

        elif "help" in user_input:
            print("Chatbot: Sure! I can answer basic questions. Try asking about my name or how I'm doing.")

        elif user_input in ["bye", "exit", "quit"]:
            print("Chatbot: Goodbye! Have a nice day.")
            break

        else:
            print("Chatbot: I'm sorry, I didn't understand that.")

# Run the chatbot
chatbot()
