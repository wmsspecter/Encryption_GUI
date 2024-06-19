 Encryption_GUI
An encryption GUI written in Python code.
I got the idea for this program from a demonstration on instagram page for various python projects. For this kind of project, I like to take the program itself and write out an algorthim explaining the code that is being written. Once I have the algorthim written out, then I go back and build the program itself using just the algorthim. 
Nice little mental exercise. ;)
# Algorithim included:

Initialize the Main Screen
 Import necessary libraries (tkinter, messagebox, base64).
Define the main_screen function to create the main GUI window.
Set window dimensions and title.
Add a label prompting the user to enter text for encryption/decryption.
Add a Text widget (text1) for user input.
 Add a label prompting the user to enter a secret key.
 Add an Entry widget (code) for secret key input, with masked characters (show="*").
 Add ENCRYPT, DECRYPT, and RESET buttons with corresponding commands (encrypt, decrypt, reset).
 Define the encrypt Function

 Retrieve the password from the code entry.
 Check if the password is "1234".
 If correct:
 Create a new top-level window for encryption results.
 Retrieve the message from text1.
 Encode the message to ASCII and then to base64.
 Decode the base64-encoded bytes back to ASCII.
 Display the encrypted message in a new Text widget.
 If the password is empty, show an error message.
 If the password is incorrect, show an error message.
 Define the decrypt Function

 Retrieve the password from the code entry.
 Check if the password is "1234".
 If correct:
 Create a new top-level window for decryption results.
 Retrieve the message from text1.
 Encode the message to ASCII and then decode from base64.
 Decode the base64-decoded bytes back to ASCII.
 Display the decrypted message in a new Text widget.
 If the password is empty, show an error message.
 If the password is incorrect, show an error message.
 Define the reset Function

 Clear the code entry and text1 content.
 Run the Main Loop

 Call main_screen to start the Tkinter main loop.
