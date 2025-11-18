# Spelling Master - GUI (Tkinter)

![Spelling Master Banner](assets/loading.png)

## 📝 Overview

**Spelling Master** is a fun and interactive desktop game to sharpen your spelling skills! Built using Python's Tkinter for the GUI, it challenges players to spell words correctly, playing audio sounds for each word and giving instant feedback on accuracy. The game is perfect for students, educators, or anyone looking to improve their English spelling in an engaging way.

---

## ✨ Features

- 🎵 **Pronunciation Audio:** Uses [gTTS](https://pypi.org/project/gTTS/) for word pronunciation and `pygame` for playback.
- 👦 **Personalized Play:** Players can enter their name and track their score.
- 🎮 **User-Friendly Interface:** Attractive, fullscreen GUI with visual feedback for each attempt.
- 🎯 **Scoreboard:** Real-time scoring system to keep you motivated.
- 📂 **Custom Word Sets:** Words are loaded from a CSV dataset (`archive/easy_set.csv`).
- 📦 **Offline Play:** Pre-generated audio for words ensures you can play even without an internet connection.

---

## 📸 Screenshots

![Game Screenshot](assets/gamebg.png)

---

## 🚀 Getting Started

### 1. **Clone the Repository**

```bash
git clone https://github.com/Umakantamaharana/spelling-master-gui-tkinter.git
cd spelling-master-gui-tkinter
```

### 2. **Install Requirements**

It's recommended to use a virtual environment.

```bash
pip install -r requirements.txt
```

#### Main Dependencies

- [Tkinter](https://wiki.python.org/moin/TkInter)
- [pygame](https://pypi.org/project/pygame/)
- [gTTS](https://pypi.org/project/gTTS/)
- [english-words](https://pypi.org/project/english-words/)

### 3. **Prepare Audio Files**

To generate audio pronunciation files for all words in your word set, run:

```python
python sm.py
```

*(The `makeaudiofiles` method will be called automatically as you play, or you can uncomment the `readcsvdataset` call in the script to pre-generate them.)*

### 4. **Run the Game**

```bash
python sm.py
```

---

## 🗂 Directory Structure

```
spelling-master-gui-tkinter/
│
├─ assets/                   # UI images and icons
│   ├─ loading.png
│   ├─ gamebg.png
│   ├─ right.png
│   └─ wrong.png
│
├─ archive/
│   └─ easy_set.csv          # Word list (one word per row)
│
├─ tmp/                      # Audio files (.mp3) generated for words
│
├─ sm.py                     # Main application script
├─ requirements.txt
└─ README.md                 # This file
```

---

## ⚙️ Customization

- **Change Word List:** Modify `archive/easy_set.csv` to use your own words.
- **Assets:** Replace images in `assets/` for a more personalized look.
- **Difficulty:** Adjust the number of words or frequency in the code to make the game more challenging.

---

## 🏆 Contributing

Contributions are welcome! If you have ideas for new features, improved UI/UX, or want to add more word sets, please open an issue or submit a pull request.

---

## 🤝 Acknowledgements

- [Google Text-to-Speech (gTTS)](https://pypi.org/project/gTTS/)
- [pygame](https://pypi.org/project/pygame/)
- [english-words](https://github.com/dwyl/english-words)
- All contributors and users!

---

## 📜 License

This project is licensed under the MIT License.

---

Enjoy improving your spelling with **Spelling Master**! 🚀