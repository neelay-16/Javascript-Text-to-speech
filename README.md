# Javascript-Text-to-speech
This is a simple Text to Speech Converter web application that allows you to convert text into speech. You can use it to listen to the text you enter.

# Preview

https://github.com/neelay-16/Javascript-Text-to-speech/assets/135517502/80876236-7b91-4334-bc6d-7433ef6f215a

# Description 
This part sets up the basic structure of an HTML document, including the <head> section for metadata and the <body> section where the visible content of the webpage is placed.

![image](https://github.com/neelay-16/Javascript-Text-to-speech/assets/135517502/93747347-92d9-4e17-a185-18aae06bb75e)


These lines create an title with the text "Text to Speech Converter" and a <textarea> element. The <textarea> is where users can input the text they want to convert to speech. It has an id attribute of "textInput" that allows JavaScript to reference this element.


![image](https://github.com/neelay-16/Javascript-Text-to-speech/assets/135517502/41ffecae-a12e-4829-a8f1-519c342b3ae0)

This line creates a <button> element with the text "Submit" and an id attribute of "submitBtn." This button will trigger the text-to-speech conversion when clicked.

![image](https://github.com/neelay-16/Javascript-Text-to-speech/assets/135517502/e13a7dff-d74c-485d-beaa-c38a3a8ada80)


This script section contains JavaScript code that adds functionality to the HTML elements.

const submitBtn = document.getElementById("submitBtn"); and const textInput = document.getElementById("textInput"); retrieve references to the HTML elements with the specified IDs ("submitBtn" and "textInput"). These references allow JavaScript to interact with these elements.

submitBtn.addEventListener("click", () => { ... }); adds a click event listener to the "Submit" button. When the button is clicked, the code inside the curly braces { ... } will be executed.

Inside the event listener:

const text = textInput.value; retrieves the value entered in the text area and stores it in the text variable.

if (text) { ... } checks if there is any text entered by the user. If there is text (i.e., the text variable is not empty), the code inside the if block will execute.

const utterance = new SpeechSynthesisUtterance(text); creates a new SpeechSynthesisUtterance object, which represents the text to be spoken. The text variable contains the user's input.

window.speechSynthesis.speak(utterance); uses the Web Speech API to speak the text represented by the utterance object. This will make the browser convert the text to speech and play it.

![image](https://github.com/neelay-16/Javascript-Text-to-speech/assets/135517502/2362dbd2-c856-4eae-903f-3be9cf3cbada)

