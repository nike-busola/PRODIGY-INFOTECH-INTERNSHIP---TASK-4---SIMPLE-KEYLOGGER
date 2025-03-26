Purpose & Functionality: This script is designed as a basic keylogger for educational purposes. It captures keystrokes using the pynput library, logs them to a file with a timestamp, and runs for a user-specified duration.

Key Components: Keylogging Function: The keylogger function is called each time a key is pressed. It captures the key (using a try/except to handle both regular characters and special keys) and writes the event with a timestamp to a log file (keylogger_log.txt).

Disclaimer & User Consent: Before starting, the script prints a detailed disclaimer outlining the ethical and legal considerations. It then asks the user to accept these terms. If the user doesn’t accept, the program exits immediately.

Duration Input: The script asks for the duration (in seconds) during which it should log keystrokes. It then converts this input into an integer and runs the keylogger for that period.

Listener Setup & Execution: A pynput.keyboard.Listener is started in the background to capture keystrokes. The script uses a while loop (with a simple time.sleep(1)) to keep the program running until the specified duration has passed, after which the listener is stopped
