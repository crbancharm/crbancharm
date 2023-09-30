import tkinter as tk

class CrazyDogApp:
    def __init__(self):
        self.coins = 20000000

    def earn_coins(self, amount):
        self.coins += amount
        self.update_coin_label()

    def update_coin_label(self):
        coin_label.config(text=f"Coins: {self.coins}")

    def play_game(self):
        # Simulate playing a game and earning coins
        self.earn_coins(10)
        game_log.config(text="You played the Crazy Dog game and earned 10 coins!")

app = tk.Tk()
app.title("Crazy Dog App")

crazy_dog = CrazyDogApp()

coin_label = tk.Label(app, text=f"Coins: {crazy_dog.coins}")
coin_label.pack()

earn_button = tk.Button(app, text="Play Game and Earn Coins", command=crazy_dog.play_game)
earn_button.pack()

game_log = tk.Label(app, text="")
game_log.pack()

app.mainloop()import tkinter as tk

class CrazyDogApp:
    def __init__(self):
        self.coins = 0

    def earn_coins(self, amount):
        self.coins += amount
        self.update_coin_label()

    def update_coin_label(self):
        coin_label.config(text=f"Coins: {self.coins}")

    def play_game(self):
        # Simulate playing a game and earning coins
        self.earn_coins(10)
        game_log.config(text="You played the Crazy Dog game and earned 10 coins!")

app = tk.Tk()
app.title("Crazy Dog App")

crazy_dog = CrazyDogApp()

coin_label = tk.Label(app, text=f"Coins: {crazy_dog.coins}")
coin_label.pack()

earn_button = tk.Button(app, text="Play Game and Earn Coins", command=crazy_dog.play_game)
earn_button.pack()

game_log = tk.Label(app, text="")
game_log.pack()

app.mainloop()
