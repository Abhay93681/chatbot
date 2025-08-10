# Enhanced Rule-Based Chatbot (Task 4 - CodeAlpha)

def chatbot():
    responses = {
        "hello": "Hi there! 👋",
        "hi": "Hello!",
        "how are you": "I'm doing great, thanks for asking! How about you?",
        "bye": "Goodbye! Have a nice day!",
        "goodbye": "See you later!",
        "what is your name": "I'm your friendly chatbot.",
        "who made you": "I was created by a Python programmer!",
        "what can you do": "I can chat with you and answer simple questions.",
        "tell me a joke": "Why did the programmer quit his job? Because he didn't get arrays. 😂",
        "where are you from": "I live inside this computer!"
    }

    print("Chatbot: Hello! Type something to chat. Type 'bye' to exit.")

    while True:
        user_input = input("You: ").strip().lower()

        if user_input in responses:
            print("Chatbot:", responses[user_input])
            if user_input in ["bye", "goodbye"]:
                break
        elif user_input == "":
            print("Chatbot: You didn't type anything!")
        else:
            print("Chatbot: Hmm... I don't know the answer to that.")

if __name__ == "__main__":
    chatbot()
