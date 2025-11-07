# sorting_hat_game.py 🎩

print("✨ Welcome to the Sorting Hat Quiz! ✨")

# 各ハウスのスコア
gryffindor = 0
ravenclaw = 0
hufflepuff = 0
slytherin = 0

# --- Q1 ---
print("\nQ1) Do you like Dawn or Dusk?")
print("  1) Dawn")
print("  2) Dusk")
answer = int(input("Enter your answer (1-2): "))

if answer == 1:
    gryffindor += 1
    ravenclaw += 1
elif answer == 2:
    hufflepuff += 1
    slytherin += 1
else:
    print("Wrong input.")

# --- Q2 ---
print("\nQ2) When I’m dead, I want people to remember me as:")
print("  1) The Good")
print("  2) The Great")
print("  3) The Wise")
print("  4) The Bold")
answer = int(input("Enter your answer (1-4): "))

if answer == 1:
    hufflepuff += 2
elif answer == 2:
    slytherin += 2
elif answer == 3:
    ravenclaw += 2
elif answer == 4:
    gryffindor += 2
else:
    print("Wrong input.")

# --- Q3 ---
print("\nQ3) Which kind of instrument most pleases your ear?")
print("  1) The violin")
print("  2) The trumpet")
print("  3) The piano")
print("  4) The drum")
answer = int(input("Enter your answer (1-4): "))

if answer == 1:
    slytherin += 4
elif answer == 2:
    hufflepuff += 4
elif answer == 3:
    ravenclaw += 4
elif answer == 4:
    gryffindor += 4
else:
    print("Wrong input.")

# --- 結果 ---
print("\n✨ Final Scores ✨")
print("Gryffindor:", gryffindor)
print("Ravenclaw:", ravenclaw)
print("Hufflepuff:", hufflepuff)
print("Slytherin:", slytherin)

# 最もスコアが高いハウスを判定
max_score = max(gryffindor, ravenclaw, hufflepuff, slytherin)

if max_score == gryffindor:
    house = "🦁 Gryffindor"
elif max_score == ravenclaw:
    house = "🦅 Ravenclaw"
elif max_score == hufflepuff:
    house = "🦡 Hufflepuff"
else:
    house = "🐍 Slytherin"

print("\n🎉 The Sorting Hat says... You belong to", house, "!")
