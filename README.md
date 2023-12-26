import pyttsx3

def speak_text(text):
    engine = pyttsx3.init()
    engine.say(text)
    engine.runAndWait()

if __name__ == '__main__':
    while True:
        print("Welcome to RoboSpeaker created by Fahad")
        user_input = input("Enter 'q' to quit\n  enter what you want me to speak: ")
        if user_input.lower() == 'q':
            speak_text("Goodbye! Thank you for using RoboSpeaker by Fahad.")
            break
        speak_text(user_input)
