# Two-Way-Communication-System-Using-Braille-

FPGA-based two-way Braille communication system. Two users (A, B) input Braille, and the recipient receives it tactilely/visually through LED blinking. The system aims to help communication between deaf-blind and visually/hearing-impaired individuals. All logic is implemented in Verilog (HDL).


## Features
- Braille Input: Input a single Braille character using 6 Braille buttons (dot1–dot6), then confirm the character with the save switch.
- Two-Way User Switching: Toggle the sender (A=0, B=1) with a toggle button, with the current sender indicated by an LED.
- Save / Backspace / Send: Save characters, delete the previous character, and send a line via switch operations.
- Autocomplete: Compares recently entered Braille against built-in words to recommend and complete the remaining letters of a matchable word.
- Braille Reception Output (LED FSM): Sequentially blinks the transmitted line of Braille characters via LEDs so the recipient can read them.
- Text LCD Output: Converts entered Braille into characters for display, and shows the autocomplete candidate at the end of the sentence.
- TFT LCD UI: Displays a KakaoTalk-style logo and UI elements on the screen.
- Debouncing: Applies a 2FF synchronizer–based debouncer to all button and switch inputs.

