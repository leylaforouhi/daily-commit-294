def count_words_starting_with(text, letter):
    words = text.lower().split()
    letter = letter.lower()

    return sum(1 for word in words if word.startswith(letter))


if __name__ == "__main__":
    text = "Python projects provide practical programming practice"
    letter = "p"

    print("Text:", text)
    print(f"Words starting with '{letter}':",
          count_words_starting_with(text, letter))
