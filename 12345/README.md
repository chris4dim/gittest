## Παραδοτέο 2:
## manage your music library: import your music library, add tags and delete/add songs.

### Αρχικά έγινε η εγκατάσταση του beets με την παρακάτω εντολή:

## install beets
```
sudo apt-get install beets
```
### Αμέσως μετά δημιουργούμε τρείς φακέλους New_music, Old_music και New_musicDB στο ~/Music όπου στον πρώτο φάκελο θα γίνεται η διαχείριση των τραγουδιών μέσω του beets, στο δεύτερο δημιουργείται η βάση δεδομένων των τραγουδιών και ο τρίτος ειναι ο φάκελος στον οποίο είχαμε τα τραγούδια μας πριν τα εισαγουμε στο beets.

### Το επόμενο βήμα είναι στο αρχείο config.yml να γράψω τα εξής: directory: ~/Music/New_music και library: ~/Music/New_musicDB/new_library.blb. Τέλος έγραψα στο παραπάνω αρχείο για να μεταφέρονται όλα τα αρχεία της μουσικής και όχι να αντιγράφονται για εξοικονόμηση χώρου: import: move:yes copy:no.


## Asciinema URL: https://asciinema.org/a/XTiUpcuhomySFsQyTEOXMsMby


## Εισαγωγή μουσικής στη βιβλιοθήκη
```
beet import ~/Music/Old_music
```                       
## add tags
```
beet modify Deep Purple artists="DP"
```                       
## add songs
```
beet move -d /home/christos title:'Haunted'
```                       
## delete songs
```
beet remove title:'Haunted'
```                       