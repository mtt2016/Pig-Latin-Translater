sentence = input("Enter a sentence/word: ")
words = sentence.split()
result = []

for word in words:
    x = word.lower()
    if x[0] in "aeiou":
        x += "way"
    else:
        first_letter = x[0]
        x = x[1:] + first_letter + "ay"
    result.append(x)

print(" ".join(result))
