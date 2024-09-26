# **Evil Taps: Custom Decks Guide**

Evil Taps allows users to import custom decks of cards to personalize their game. Follow this guide to create, host, and import your own deck into the app.

## **Table of Contents**
1. [Deck Format](#deck-format)
2. [Creating a Custom Deck](#creating-a-custom-deck)
3. [Hosting the Deck](#hosting-the-deck)
4. [Importing the Deck](#importing-the-deck)
5. [Example Deck](#example-deck)

---

## **Deck Format**

A custom deck consists of two types of cards:
- **White Cards**: These are responses.
- **Black Cards**: These are prompts with one or more blanks for responses.

The deck file must be written in **JavaScript-like format** and follow this structure:

```js
let whiteCardResponses = [
    "Your first response.",
    "Another witty reply.",
    "Something completely random."
];

let blackCardResponses = [
    "_ is the reason I can't sleep at night.",
    "If I had a dollar for every _, I'd be rich.",
    "Next on my bucket list: _."
];
```

- The **whiteCardResponses** array contains strings for the response cards.
- The **blackCardResponses** array contains strings for the prompt cards. Use underscores (`_`) to indicate blanks.

---

## **Creating a Custom Deck**

1. **Open a Text Editor**: You can use any text editor (e.g., Visual Studio Code, Notepad++, or even a basic notepad).
2. **Follow the Deck Format**: Copy the deck format from above and replace the example cards with your custom responses and prompts.
3. **Save Your Deck**:
   - Save the file as `YourDeckName.deck`.
   - Make sure the file extension is `.deck`, as the app only accepts this format for import.

---

## **Hosting the Deck**

To import a custom deck into Evil Taps, the deck file must be hosted online. Here are some ways to host your `.deck` file:

### **Option 1: GitHub**
1. **Create a Public Repository**: You can upload your `.deck` file to a public GitHub repository.
2. **Get the Raw File URL**:
   - Navigate to your deck file in your GitHub repository.
   - Click on the "Raw" button to get the raw file URL. It should look something like this:
     ```
     https://raw.githubusercontent.com/username/repo/main/YourDeckName.deck
     ```

### **Option 2: Dropbox**
1. **Upload the File to Dropbox**.
2. **Share the File**:
   - Get the shareable link and replace the `?dl=0` at the end of the URL with `?dl=1`.
   - Example:
     ```
     https://www.dropbox.com/s/filename.deck?dl=1
     ```

### **Option 3: Google Drive**
1. **Upload the Deck to Google Drive**.
2. **Make the File Public**: Set the sharing permissions to “Anyone with the link.”
3. **Get the Direct Download Link**:
   - Use the file ID to create a direct download link in this format:
     ```
     https://drive.google.com/uc?export=download&id=FILE_ID
     ```

### **Option 4: Free Hosting Services**
You can also use free file-hosting services like [file.io](https://www.file.io/) or [Pastebin](https://pastebin.com) for temporary hosting.

---

## **Importing the Deck**

1. **Open Evil Taps**.
2. **Hold to Import**: On the main screen, hold the card for 1 second to bring up the custom deck importer.
3. **Enter the URL**: Paste the URL where your `.deck` file is hosted.
4. **Load Deck**: Once you press "Load Deck," the app will fetch the custom deck and replace the default cards.

---

## **Example Deck**

Here is a sample `.deck` file that you can copy and modify for your own custom deck:

```js
let whiteCardResponses = [
    "Tweeting without thinking.",
    "Doing Kegels at work.",
    "Duct taping my life together.",
    "Drinking wine from a mug.",
    "Pretending to understand NFTs."
];

let blackCardResponses = [
    "_ is the new black.",
    "If I had a nickel for every time I _, I'd be broke.",
    "_ is the best way to get fired.",
    "Life's greatest mystery: _.",
    "The secret to happiness is _."
];
```


---

## **Troubleshooting**
- **File not loading**: Make sure the URL points directly to the raw `.deck` file.
- **Invalid format**: Double-check the syntax in your `.deck` file. Both `whiteCardResponses` and `blackCardResponses` arrays must be properly formatted.
- **Deck not updating**: Ensure the deck URL is correct and the file is publicly accessible.

For more help, reach out to us at [nawras@smol.date](mailto:nawras@smol.date).
