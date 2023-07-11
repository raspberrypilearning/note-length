Il existe plusieurs façons de régler la durée d'une note.

**Utiliser une valeur pour définir la durée d'une seule note**

Lorsque tu joues une seule note, tu peux décider de sa durée en saisissant une valeur pour le deuxième argument.

Le `0,1` dans l'exemple de code ci-dessous jouera la note pendant 0,1 seconde.

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 
line_highlights: 
---
haut_parleur.play(c_note, 0.1) # joue le do du milieu (middle c) pendant 0,1 seconde
--- /code ---

**Utiliser une constante pour la durée d'une seule note**

Tu peux remplacer la valeur du deuxième argument par une constante.

L'exemple ci-dessous utilise la constante `RYTHME`. Cela peut ensuite être utilisé pour régler le rythme de n'importe quel morceau de ton programme.

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 
line_highlights: 
---
RYTHME = 1 # constante

haut_parleur.play(c_note, RYTHME) # joue le do du milieu (middle c) pendant 1 seconde
--- /code ---

**Définir la durée de chaque note d'un morceau à l'aide d'une valeur**

Si tu veux jouer un morceau, tu dois utiliser une liste pour stocker toutes les notes de ton morceau avec la durée de chaque note.

L'exemple ci-dessous montre une liste de listes. Chaque liste contient une note entre guillemets `''` puis une valeur pour la durée que la note doit jouer.

--- code ---
---
language: python
filename: 
line_numbers: false
line_number_start: 1
line_highlights: 
---

mon_son = [ ['d5', 1], ['d#5', 0.5], ['f5', 1.2]] # les notes, ainsi que la longueur de chaque note

--- /code ---

**Définir la durée de chaque note d'un morceau à l'aide d'une constante**

L'exemple ci-dessous définit la constante `RYTHME` sur 0,4 sur la ligne 1.

Tu peux alors voir une liste de listes sur la ligne 3. Chaque liste contient une note entre guillemets `''` puis la constante `RYTHME`.

--- code ---
---
language: python
filename: 
line_numbers: true
line_number_start: 1
line_highlights: 
---
RYTHME = 0.4 # The length of a note in a single beat

mon_son = [ ['d5', RYTHME], ['d#5', RYTHME / 2], ['f5', RYTHME * 1.5]] # La durée d'une note sur un seul temps

--- /code ---

Tu peux rendre la note **plus courte** en divisant le temps : `RYTHME / 2`.

Tu peux rendre la note **plus longue** en multipliant le temps : `RYTHME * 1.5`

**Astuce :** Cette option te permet de définir le BPM de ton morceau et de l'ajuster en fonction de tes besoins.

