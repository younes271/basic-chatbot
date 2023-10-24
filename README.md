# basic-chatbot
A new repository created via Python script


---

```python
import random

GREETING_KEYWORDS = ("hello", "hi", "greetings", "what's up",)

GREETING_RESPONSES = ["hi", "hey", "*nods*", "hi there", "hello"]

def check_for_greeting(sentence):
    for word in sentence.split():
        if word.lower() in GREETING_KEYWORDS:
            return random.choice(GREETING_RESPONSES)

def main():
    print("Hello! I am a chatbot. Start a conversation with me!")
    while True:
        user_input = input("> ")
        print(check_for_greeting(user_input))

if __name__ == "__main__":
    main()
```
This is a very basic chatbot that only responds to greetings. To make it more advanced, you would need to use natural language processing techniques, which is outside the scope of this simple example.