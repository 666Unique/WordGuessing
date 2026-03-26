# Word Guessing Game

A simple web-based word guessing game for teachers to use with students.

## What is this?

This is a simple website that helps students learn vocabulary by displaying words and testing their knowledge of definitions. Teachers can customize the number of words and time limit for each guess.

## How to Use

### Starting the Game

1. **Open terminal/command prompt** and navigate to the project folder:
   ```
   cd c:\ADisk\Project\WordGuessing
   ```
   
2. **Start the web server** (IMPORTANT: Must run from the project directory!):
   ```
   python -m http.server 8000
   ```
   
3. **Open your browser** and go to: `http://localhost:8000`

⚠️ **Important:** The server must be started from the project directory where `index.html` and `Words.xlsx` are located, otherwise you'll see a directory listing instead of the website.

### Playing the Game

1. **Set the number of words**: Enter how many words you want to test (default: 5)
2. **Set the time limit**: Enter how many seconds students have to guess each word (default: 30)
3. **Click "Start Game"** to begin
4. **Students guess the word** displayed on screen
5. **Click "Show Definition"** to reveal the answer
6. **Click "Next Word"** to move to the next word
7. **Click "Quit Game"** to exit early and return to settings

### Updating Word List

To add or change words:
1. Open `Words.xlsx` in Excel or Google Sheets
2. Keep two columns: `Word` and `Description`
3. Add your words in the first column and definitions in the second column
4. Save the file

## Features

- ✅ Random word selection from Excel file
- ✅ Customizable number of words
- ✅ Customizable time limit per word
- ✅ Countdown timer
- ✅ Show/hide definition button
- ✅ Progress indicator
- ✅ Quit game button to return to settings
- ✅ Simple, clean interface

## Files

- `index.html` - The main website file (all code in one file)
- `Words.xlsx` - Excel file containing words and definitions
- `README.md` - This file

## Technical Details

This project uses:
- **HTML5** - Structure of the website
- **CSS** - Styling and layout
- **JavaScript** - Game logic and interactivity
- **SheetJS (xlsx)** - Library to read Excel files in the browser
- **Python HTTP Server** - To serve files locally

All code is contained in a single HTML file with inline CSS and JavaScript, making it easy for year 11-13 students to understand and modify.

## For Teachers

This tool is designed to be simple and easy to use:
- No installation required (just Python for the web server)
- Works offline once files are downloaded
- Easy to customize by editing the Excel file
- Simple code that students can learn from

## Troubleshooting

**Problem**: Words not loading
- Make sure `Words.xlsx` is in the same folder as `index.html`
- Check that the Excel file has columns named `Word` and `Description`
- Ensure you're accessing the site via `http://localhost:8000` (not opening the file directly)

**Problem**: Server won't start
- Make sure Python is installed on your computer
- Try running `python3 -m http.server 8000` instead
- Check that port 8000 is not being used by another program

## License

Free to use and modify for educational purposes.