There are several ways to set the length of a note. 

### Use a value to set the length of a single note

When you play a single note you can decide how long it will play for by entering a value for the second argument. 

The `0.1` in the example code below will play the note for 0.1 seconds. 

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 
line_highlights: 
---
speaker.play(c_note, 0.1) # play the middle c for 0.1 seconds
--- /code ---

### Use a constant for the length of a single note

You can replace the value in the second argument with a constant.

The example below uses the constant `BEAT`. This can then be used to set the beat for any tune in your program.

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 
line_highlights: 
---
BEAT = 1 # a constant

speaker.play(c_note, BEAT) # play the middle c for 1 second
--- /code ---

### Set the length of each note in a tune using a value

If you want to play a tune then you should use a list to store all of the notes in your tune along with the length of each note. 

The example below shows a list of lists. Each list contains a note in quotes `''` and then a value for the length the note should play. 

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 1
line_highlights: 
---

my_tune = [ ['d5', 1], ['d#5', 0.5], ['f5', 1.2]] # the notes, along with the length of each note

--- /code ---

### Set the length of each note in a tune using a constant

The example below sets the `BEAT` constant to 0.4 on line 1. 

You can then see a list of lists on line 3. Each list contains a note in quotes `''` and then the `BEAT` constant. 

--- code ---
---
language: python
filename: 
line_numbers: true
line_number_start: 1
line_highlights: 
---
BEAT = 0.4 # The length of a note in a single beat

my_tune = [ ['d5', BEAT], ['d#5', BEAT / 2], ['f5', BEAT * 1.5]] # the notes, along with the length of each note

--- /code ---

You can make the note **shorter** by dividing the beat: `BEAT / 2`.

You can make the note **longer** by multiplying the beat: `BEAT * 1.5`

**Tip:** This option allows you to set the BPM of your tune and adjust it to suit your needs.

