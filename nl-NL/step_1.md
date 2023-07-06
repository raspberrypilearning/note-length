Er zijn verschillende manieren om de lengte van een noot in te stellen.

**Gebruik een waarde om de lengte van een enkele noot in te stellen**

Als je een enkele noot afspeelt, kun je bepalen hoe lang deze wordt afgespeeld door een waarde in te voeren voor de tweede parameter.

The `0.1` in the example code below will play the note for 0.1 seconds.

--- code ---
---
language: python filename: line_numbers: false line_number_start:
line_highlights:
---
speaker.play(c_note, 0.1) # play the middle c for 0.1 seconds --- /code ---

**Gebruik een constante voor de lengte van een enkele noot**

Je kan de waarde van de tweede parameter vervangen door een constante.

In het onderstaande voorbeeld wordt de constante `BEAT`gebruikt. Dit kan vervolgens worden gebruikt om de slag in te stellen voor elk deuntje in je programma.

--- code ---
---
language: python filename: line_numbers: false line_number_start:
line_highlights:
---
BEAT = 1 # a constant

speaker.play(c_note, BEAT) # play the middle c for 1 second --- /code ---

**Stel de lengte in van elke noot van een liedje met behulp van een waarde**

Als je een melodie wilt spelen, moet je een lijst gebruiken om alle noten van je liedje in op te slaan, samen met de lengte van elke noot.

Het onderstaande voorbeeld toont een lijst met lijsten. Elke lijst bevat een noot tussen aanhalingstekens `''` en vervolgens een waarde voor de lengte die de noot moet spelen.

--- code ---
---
language: python filename: line_numbers: false line_number_start: 1
line_highlights:
---

my_tune = [ ['d5', 1], ['d#5', 0.5], ['f5', 1.2]] # the notes, along with the length of each note

--- /code ---

**Stel de lengte van elke noot in een melodie in met behulp van een constante**

The example below sets the `BEAT` constant to 0.4 on line 1.

You can then see a list of lists on line 3. Elke lijst bevat een noot tussen aanhalingstekens `''` en vervolgens de constante `BEAT`.

--- code ---
---
language: python filename: line_numbers: true line_number_start: 1
line_highlights:
---
BEAT = 0.4 # The length of a note in a single beat

my_tune = [ ['d5', BEAT], ['d#5', BEAT / 2], ['f5', BEAT * 1.5]] # the notes, along with the length of each note

--- /code ---

Je kunt de noot **korter** maken door de slag te delen: `BEAT / 2`.

Je kunt de noot **langer** maken door de slag te vermenigvuldigen: `BEAT * 1.5`

**Tip:** Met deze optie kun je de BPM van je deuntje instellen en aanpassen aan je behoeften.

