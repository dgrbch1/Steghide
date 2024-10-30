
# Steganography Tutorial Website

This project is a simple HTML/CSS website that demonstrates how to use **steghide** to embed and extract hidden messages from images. The tutorial provides step-by-step instructions, accompanied by screenshots and a GIF to visually illustrate the process.

## Table of Contents

- [Overview](#overview)
- [Screenshots](#screenshots)
- [GIF Summary](#gif-summary)
- [How to Run the Project](#how-to-run-the-project)
- [Technologies Used](#technologies-used)
- [Instructions](#instructions)
- [License](#license)

---

## Overview

The purpose of this website is to provide a visual guide on using **steghide**, a steganography tool that allows you to hide files within images. This can be useful for hiding sensitive information in plain sight. The website showcases the following steps:
1. Embedding a text file into an image.
2. Verifying the embedded data in the image.
3. Extracting the hidden text from the image.
4. Displaying the extracted message.

## Screenshots

### Step-by-Step Guide

1. **Embedding Data into an Image**
   - ![Embedding Data](./confuse.png
     
   - Command: `steghide embed -cf cvr.jpg -ef emb.txt`

2. **Checking the Embedded Data**
   - ![Checking Embedded Data](./all.png)
   - Command: `steghide info cat.jpg`

3. **Extracting the Hidden Message**
   - ![Extracting Message](./decryption.png)
   - Command: `steghide extract -sf cat.jpg -xf embeddedmessage.txt`

4. **Viewing the Extracted Message**
   - ![Viewing Extracted Message](./chatbot.png)
   - Command: `cat embeddedmessage.txt`

## GIF Summary

To provide a quick overview of the process, a GIF is included to demonstrate the entire workflow from embedding to extracting a message.
![Steganography Process GIF](./Animation3.gif)

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/steganography-tutorial-website.git
   ```
2. Open the `index.html` file in your browser to view the website.

## Technologies Used

- **HTML**: Structuring the content.
- **CSS**: Styling and layout of the tutorial sections.
- **Steghide**: A command-line tool for steganography, used to embed and extract hidden files within images.

## Instructions

To follow this tutorial, you’ll need to have **steghide** installed on your system. Here’s a summary of the commands used in this project:

1. **Embed a Text File**:
   ```bash
   steghide embed -cf cvr.jpg -ef emb.txt
   ```
   This command hides `emb.txt` inside `cvr.jpg`.

2. **Verify Embedded Data**:
   ```bash
   steghide info cat.jpg
   ```
   This command checks if there’s hidden data in `cat.jpg`.

3. **Extract Hidden Data**:
   ```bash
   steghide extract -sf cat.jpg -xf embeddedmessage.txt
   ```
   This command extracts the hidden file as `embeddedmessage.txt` from `cat.jpg`.

4. **Display Extracted Message**:
   ```bash
   cat embeddedmessage.txt
   ```
   This command shows the content of the extracted file.

## License

This project is open source and available under the [MIT License](LICENSE).


