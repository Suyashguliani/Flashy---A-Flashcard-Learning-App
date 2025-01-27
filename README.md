# Flashy---A-Flashcard-Learning-App
Flashy is a simple flashcard-based learning application built using Python's Tkinter library. It allows users to learn French vocabulary by flipping through flashcards and marking words they already know. The application dynamically saves progress, so users can continue learning from where they left off.
Features

Flashcard Learning: View French words on the front of the card and their English translations on the back.

Progress Tracking: Automatically saves words the user knows and removes them from the learning deck.

Dynamic Updates: Updates the flashcard deck based on user interaction.

Beautiful UI: Simple and intuitive user interface designed with Tkinter.

Project Structure

.
├── data
│   ├── french_words.csv          # Initial vocabulary file
│   ├── words_to_learn.csv        # Dynamically updated vocabulary file
├── images
│   ├── card_front.png            # Front side of the flashcard
│   ├── card_back.png             # Back side of the flashcard
│   ├── right.png                 # Image for the 'Known' button
│   ├── wrong.png                 # Image for the 'Unknown' button
├── main.py                       # Main script for the application
└── README.md                     # Project documentation

How It Works

The application reads a dataset of French words (french_words.csv) to create flashcards.

If a progress file (words_to_learn.csv) exists, the application uses it to load the remaining words. Otherwise, it starts with the full dataset.

Users can:

Mark words as known: Removes the word from the deck and saves progress.

Skip words: Keeps the word in the deck for future review.

After 3 seconds, the card flips to reveal the English translation of the word.

Prerequisites

Python 3.x

Required libraries:

pandas

tkinter (built-in with Python)

Installation

Clone the repository:

git clone https://github.com/Suyashguliani/flashy.git
cd flashy

Install dependencies:

pip install pandas

Ensure the data folder contains french_words.csv and the images folder contains the required images.

Usage

Run the application:

python main.py

Use the flashcards to learn French words:

Press the tick button (✔️) if you know the word.

Press the cross button (❌) if you don't know the word.

Flashcard Front:
Displaying a French word.

Flashcard Back:
Revealing the English translation after 3 seconds.

Acknowledgements

This project is inspired by Angela Yu's 100 Days of Code course. Special thanks to her for the excellent resources and guidance.

License

This project is licensed under the MIT License. Feel free to use and modify it as needed.

Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.
