Python program to build flashcard using class in Python

class flashcard:
    def __init__(self,word,meaning):
        self.word=word
        self.meaning=meaning
    def __str__(self):
        return self.word + '('+self.meaning+')'
flash=[]
print("Welcome! to FlashCard Game")
while True:
    word=input("Enter the name you want create for flashcard: ")
    meaning=input("Enter the meaniing of a flashcard: ")
    flash.append(flashcard(word,meaning))
    option=int(input("Enter 0 For new entry of flashcard: "))

    if(option):
        break

print("\nYour Flashcards")
for i in flash:
    print("> ",i)
