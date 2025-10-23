# Passphrase Generator
A simple, single-page web application to generate secure, random passphrases. It provides both an on-page generator and a convenient bookmarklet that copies a new passphrase to your clipboard on any website.  
  
This tool is built with vanilla JavaScript and contains no external dependencies beyond [Tailwind CSS](https://tailwindcss.com/) for styling, ensuring transparency and security. 
  
All passphrase generation happens 100% client-side.  

## Live Demo  
You can use the live version of this tool hosted on GitHub Pages:  
[https://danlibbo.github.io/passphraseGenerator/](https://danlibbo.github.io/passphraseGenerator/)

## Features
* **On-Page Generator**: Instantly create and copy a new passphrase directly from the webpage.  
* **Bookmarklet**: Add the generator to your browser's bookmarks/favourites bar for use on any webpage.  
* **High Entropy**: Generates passphrases from large, curated, and SFW (safe-for-work) word lists.  
* **Secure & Transparent**: 100% client-side vanilla JavaScript. No data is ever sent to any server.  
* **Informative UI**: The page explains the generation logic and shows the full, readable source code.

## How to Use
There are two ways to use this tool.
1. **On-Page Generator**
    1. Visit [the live demo page](https://danlibbo.github.io/passphraseGenerator/).  
    2. Click the "Generate Passphrase" button.  
    3. Click the copy icon to copy the new passphrase to your clipboard.  
2. **The Bookmarklet** (Recommended)  
    1. This is the most powerful feature. It lets you generate a passphrase on any website (e.g., a new account sign-up form) without having to open a new tab.  
    2. Visit [the live demo page](https://danlibbo.github.io/passphraseGenerator/).  
    3. Find the green button labelled "Drag to Bookmarks →".  
    4. Click and drag this button up to your browser's bookmarks bar (also called the "favourites bar").
       
That's it! Now, when you are on any website and need a new password, just click that bookmark. A new passphrase will be instantly generated and copied to your clipboard.

## Passphrase Structure
Each passphrase follows a consistent, random format:  
`[Descriptor] + [Punctuation 1] + [Verb] + [Puncutation 2] + [Noun] + [Number]`  
  
Example: `Quickly#Driving.List42`  
  
**Capitalisation**: The first letter of each word is randomly capitalised (or lowercased). The logic ensures that at least one of the three words will be capitalised.  

**Word Lists**: The generator pulls from three curated, SFW lists:  
  * 147 Descriptors (adjectives/adverbs)  
  * 173 Verbs (present/past participles)  
  * 100 Nouns
  
**Punctuation**: A random choice from `!, #, $, %, &, *, +, -`  

**Number**: A random two-digit number from 10 to 99.

## Technology Used
HTML5  
Tailwind CSS  
Vanilla JavaScript (ES6+)  

## License
Distributed under the MIT License. Copyright (c) 2025 Dan Libbesson
