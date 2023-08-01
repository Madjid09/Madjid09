from textblob import TextBlob

def correct_spelling(text):
    # Create a TextBlob object
    blob = TextBlob(text)

    # Correct spelling errors
    corrected_text = blob.correct()

    return str(corrected_text)

if __name__ == "__main__":
    # Get input text from the user
    input_text = input("Enter the text with spelling errors: ")

    # Correct the spelling errors
    corrected_text = correct_spelling(input_text)

    # Display the corrected text
    print("Corrected text:")
    print(corrected_text)
