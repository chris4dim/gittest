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

---


## Παραδοτέο 3:
## Download a torrent


## install rtorrent
```
sudo apt-get install rtorrent
```                                             
### Το επόμενο βήμα ήταν να κατεβάσω το αρχείο .rtorrent.rc από το github:
```
https://gist.github.com/bryanjswift/1525912
```            

### Στο επόμενο βήμα δημιούργησα 3 φακέλους rDownloads, rSessions και rWatch στο /home/christos/. Μετά άλλαξα τον φάκελο αποθήκευσης μέσα στο αρχείο .rtorrent.rc τον φάκελο αποθήκευσης απο unsorted σε /home/christos/Downloads.



## Asciinema URL: https://asciinema.org/a/ndwwRGIYdskvSX66YSVdI0wpi


---

## Παραδοτέο 4:
## Visualize an mp3: demonstrate album art and visualizations with an mp3 player and various songs.

## install cmus
```
sudo apt-get install cmus

```                       
### Η χρήση του cmus δίνει τη δυνατότητα στον χρήστη να διαχειριστεί πλήθος αρχείων mp3, να τα ταξινομήσει με βάση τα album και δημιουργήσει playlists της επιλογής του. Η εμφάνιση είναι απλή και είναι χωρισμένο σε 7 διαφορετικές εμφανίσεις (views) όπου η κάθε εμφάνιση επιλέγετα με βάση έναν αριθμό από το 1-7:

```
1. Library
2. Sorted Library
3. Playlist
4. Play Queue
5. Browser
6. Filters
7. Settings
```           
## Εισαγωγή mp3 στο cmus:
```
:add ~/Music

```           

## Asciinema URL: https://asciinema.org/a/rk8NkeNtKJ8s3HKKkeRyCxEv3


## Κάποια βασικά keybindings είναι:

```
x = play song
c = pause
v = stop
z = previous song
b = next song

```           


---

## Παραδοτέο 5
## Watch video: youtube video streaming.

## install mpv
### Για την εγκαστάσταση του mpv έγινε η χρήση των παρακάτω εντολών:

```
sudo add-apt-repository ppa:mc3man/mpv-tests
sudo apt-get update
sudo apt-get install mpv

```       
## Asciinema URL:https://asciinema.org/a/3Z7CzQgc2m8EHAwPMtaM2WvsG

### Η εκτέλεση του βίντεο γίνεται με την παρακάτω εντολή:

```
mpv "link"

```       
# Μάθημα: Πολυμέσα - Τελική Αναφορά
# Όνομα: Χρήστος
# Επίθετο: Δήμας
# Α.Μ.: Π2017204
# Προφίλ Github: [Προφίλ](https://github.com/chris4dim)
# Λίνκ Αποθετηρίου: [Λίνκ Αποθετηρίου](https://github.com/chris4dim/mm/tree/2017204/projects/2017204)

### Σύνοψη:
Στο πλαίσο του μαθήματος Πολυμέσα πραγματοποιήθηκαν 5 παραδοτέα, τα οποία εκπονήθηκαν και στάλθηκαν στις αντίστοιχες ημερομηνίες που είχαν οριστεί από τον διδάσκοντα. Το 1ο παραδοτέο είχε ως θέμα την αναζήτηση, το κατέβασμα και την μετατροπή ενός τραγουδιού σε μορφή mp3 από το youtube. Το 2ο παραδοτέο είχε ως θέμα τη διαχείριση μιας μουσικής βιβλιοθήκης, που αφορά στη δημιουργία και εισαγωγή τραγουδιών σε βιβλιοθήκη, την προσθήκη "tags" σε τραγούδια, καθώς επίσης προσθήκης και αφαίρεσης τραγουδιών από τη βιβλιοθήκη. Το 3ο παραδοτέο αναφέρεται στο κατέβασμα ενός αρχείου τόρεντ. Το 4ο παραδοτέο έχει ως θέμα την επίδειξη διαχείρισης μουσικών άλμπουμ με αρχεία mp3, καθώς επίσης και "playlists". Τέλος, το 5ο παραδοτέο έχει ως αντικείμενο την παρακολούθηση ενός βίντεο απο το youtube. 

### Σύντομη Εισαγωγή:
Για να εκπονηθεί το 1ο παραδοτέο έγινε η χρήση του τέρμιναλ και η εγκατάσταση των απαραίτητων εφαρμογών, όπως youtube-dl και mpv και στη συνέχεια έγινε η αναζήτηση ενός τραγουδιού στο youtube, κατέβηκε σε μορφή mp3 και τέλος έγινε η εκτέλεσή του. Για την εκπόνηση του 2ου παραδοτέου έγινε η εγκατάσταση και η χρήση της εφαρμογής beets, όπου με τη χρήση του γίνεται η επίδειξη λειτουργίας εισάγωντας τραγούδια, αφαιρώντας και δημιουργώντας "tags". Στο 3ο παραδοτέο, γίνεται η εγκατάσταση της εφορμογής rtorrent, όπου στη συνέχεια γίνεται η επίδειξη λειτουργίας του, κατεβάζοντας ένα αρχείο τόρεντ. Το 4ο παραδοτέο εκπονήθηκε κάνοντας εγκατάσταση και χρήση της εφαρμογής cmus, όπου στη συνέχεια έγινε η επίδειξη της εφαρμογής εισάγωντας 2 αλμπουμ με τραγούδια μορφής mp3 και κάνοντας επεξεργασία των ανωτέρω αρχείων mp3 μέσω της συγκεκριμένης εφαρμογής. Τέλος, για τη διεκπαιρέωση του 5ου παραδοτέου γίνεται η χρήση του mpv και του αντίστοιχου λινκ του βίντεο που έχει επιλέξει ο χρήστης, όπως και έγινε και στην επίδειξη. 

### Σύντομη Ανάλυση σχετικών Έργων και Εργαλείων:
H εκπόνηση των ανωτέρω παραδοτέων πραγματοποιήθηκαν στο λειτουργικό Ubuntu 18.04 LTS και με τη χρήση του τέρμιναλ έγινε η διεκπαιρέωση των πέντε παραδοτέων. Αρχικά έγινε η αλλαγή του hostname του υπολογιστή και η αντικατάστασή του με τον αριθμό μητρώου μου P2017204  με την εξής εντολή: hostnamectl set-hostname P2017204. Επόμενο βήμα ήταν να γίνει η εγκατάσταση της εφαρμογής asciinema, ώστε να πραγματοποιηθεί η καταγραφή του τέρμιναλ για την επίδειξη του εκάστοτε παραδοτέου. Αφού πρώτα κατέβασα το asciinema από το github, αμέσως μετά έκανα την εγκατάσταση της εφαρμογής με την εξής εντολή: sudo apt-get install asciinema. Στη συνέχεια, πραγματοποιήθηκε η εγκαστάσταση των python και python3, όπου αποτελoύν προαπαιτούμενο για την πραγματοποίηση των απαραίτητων διεργασιών. Η εγκατάσταση πραγματοποίηθηκε με τις εξής εντολές: sudo apt-get install python και sudo apt-get install python3. Τέλος, πραγματοποιήθηκε η εγκατάσταση κάποιων απαραίτητων codecs, τα οποία ήταν απαραίτητα για το τρέξιμο των βίντεο, ώστε να λειτουργεί σωστά ο ήχος και η εικόνα. Η εγκατάσταση των ανωτέρω codecs πραγματοποιήθηκε με την παρακάτω εντολή: sudo apt-get install ffmpeg.

### Μέθοδος και Τεχνικές Ανάπτυξης:
Αρχικά, για να εκπονηθεί το 1ο παραδοτέο έπρεπε να κάνω την εγκατάσταση με την παρκάτω εντολή: sudo apt-get install youtube-dl. Στη συνέχεια κατέβασα απο το github το mpv και το έκανα εγκατάσταση με τις εξής εντολές κατά σειρά: sudo add-apt-repository ppa:mc3man/mpv-tests και sudo apt-get install mpv. Τέλος, για να κατεβάσω το τραγούδι από το youtube έχοντας τη μορφή mp3 χρησιμοποίησα την παρακάτω εντολή και εισήγαγα το λινκ του τραγουδιού: youtube-dl --extract-audio --audio-format mp3 --prefer-ffmpeg "link". Για το 2ο παραδοτέο έκανα την εγκατάσταση του beet με την παρακάτω εντολή: sudo apt-get install beets. Στη συνέχεια,  δημιούργησα τρείς φακέλους New_music, Old_music και New_musicDB στο ~/Music, όπου στον πρώτο φάκελο θα γίνεται η διαχείριση των τραγουδιών μέσω του beets, στο δεύτερο δημιουργείται η βάση δεδομένων των τραγουδιών και ο τρίτος ειναι ο φάκελος στον οποίο είχαμε τα τραγούδια μας πριν τα εισαγουμε στο beets. Το επόμενο βήμα ήταν στο αρχείο config.yml να γράψω τα εξής: directory: ~/Music/New_music και library: ~/Music/New_musicDB/new_library.blb. Τέλος έγραψα στο παραπάνω αρχείο για να μεταφέρονται όλα τα αρχεία της μουσικής και όχι να αντιγράφονται για εξοικονόμηση χώρου: import: move:yes copy:no. Μετά την υλοποίηση των παραπάνω βημάτων, η εφαρμογή ήταν έτοιμη για χρήση με τις εξής εντολές: beet import ~/Music/Old_music = εισαγωγή μουσικής στη βιβλιοθήκη, beet modify Deep Purple artists="DP" = εισαγωγή "tags", beet move -d /home/christos title:'Haunted' = εισαγωγή τραγουδιών και beet remove title:'Haunted' = διαγραφή τραγουδιών. Στο 3ο παραδοτέο, κατέβασα και έκανα  εγκατάσταση της εφαρμογής rtorrent με τις παρακάτω εντολές κατά σειρά: https://gist.github.com/bryanjswift/1525912 και sudo apt-get install rtorrent. Τέλος, δημιούργησα 3 φακέλους rDownloads, rSessions και rWatch στο /home/christos/. Μετά άλλαξα τον φάκελο αποθήκευσης μέσα στο αρχείο .rtorrent.rc, τον φάκελο αποθήκευσης απο unsorted σε /home/christos/Downloads, ώστε να αποθηκεύονται τα τόρεντς που κατεβαίνουν. Ο χειρισμός του rtorrent επιτυγχάνεται: Ctrl+s = κατεβαίνει το torrent, Ctrl+d = σταματάει το torrent, Ctrl+2xd = διαγράφεται το torrent και Ctrl+q = έξοδος από το rtorrent. Για το 4ο παραδοτέο έγινε η εγκατάσταση της εφαρμογής cmus με την παρακάτω εντολή: sudo apt-get install cmus. Η χρήση του cmus δίνει τη δυνατότητα στον χρήστη να διαχειριστεί πλήθος αρχείων mp3, να τα ταξινομήσει με βάση τα album και να δημιουργήσει playlists της επιλογής του. Η εμφάνιση είναι απλή και είναι χωρισμένο σε 7 διαφορετικές εμφανίσεις (views) όπου η κάθε εμφάνιση επιλέγετα με βάση έναν αριθμό από το 1-7. Κάποια βασικά πλήκτρα για τη χρήση της εφαρμογής είναι: x = εκτέλεση τραγουδιού, c = διάλειμα, v = διακοπή, z = προηγούμενο τραγούδι και
b = επόμενο τραγούδι. Τέλος, για τη διεκπαιρέωση του 5ου παραδοτέου, ήταν απαραίτητο το κατέβασμα και η εγκατάσταση του mpv, το οποίο είχε πραγματοποιηθεί σε προηγούμενο παραδοτέο. Για να εκτελεστεί ένα βίντεο χώρις να κατέβει στον υπολογιστή έγινε με τν παρκάτω εντολή και το αντίστοιχο λίνκ του youtube: mpv "link".

### Αποτελέσματα:
Με τη χρήση λοιπόν του asciinema έγινε η καταγραφή του τέρμιναλ στα βήματα που ακολούθησα για την πραγματοποίηση του κάθε παραδοτέου. Έτσι λοιπόν παρακάτω παραθέτω κατα σειρά τις καταγραφές, που πραγματοποιήθηκαν για το κάθε παραδοτέο:
### 1ο παραδοτέο.
## Asciinema URL: [1ο paradoteo](https://asciinema.org/a/LzIEgPe6Zvtg61N8DdWKWcqy2)
### 2ο παραδοτέο.
## Asciinema URL: [2o paradoteo](https://asciinema.org/a/XTiUpcuhomySFsQyTEOXMsMby)
### 3ο παραδοτέο.
## Asciinema URL: [3o paradoteo](https://asciinema.org/a/ndwwRGIYdskvSX66YSVdI0wpi)
### 4ο παραδοτέο.
## Asciinema URL: [4o paradoteo](https://asciinema.org/a/rk8NkeNtKJ8s3HKKkeRyCxEv3)
### 5ο παραδοτέο.
## Asciinema URL: [5o paradoteo](https://asciinema.org/a/3Z7CzQgc2m8EHAwPMtaM2WvsG)

### Συμπεράσματα:
Ακολουθώντας τα ανωτέρω βήματα, τα οποία προανέφερα παραπάνω, προγματοποίησα τα παραδοτέα με επιτυχία χρησιμοποιώντας το λειτουργικό Ubuntu και πιο συγκεκριμένα το τέρμιναλ του συγκεκριμένου λειτουργικού. Διαπίστωσα λοιπόν ότι η χρήση του είναι αρκετά εύκολη και κάνοντας εγκατάσταση του κάθε προγραμματος ανάλογα με το κάθε ζητούμενο μπορεί ο χρήστης να πραγματοποιήσει κάθε είδους εργασία με απλές εντολές. Ο χρήστης από το τέρμιναλ μπορεί πολύ εύκολα να κατεβάσει ένα αρχείο mp3 από το youtube και να το αποθηκεύσει στον υπολογιστή του. Ακόμη, ο χρήστης μπορεί να δημιουργήσει επιθυμητές βιβλιοθήκες μουσικής κάνοντας πολύ εύκολα την διαχείρισή τους, εισάγοντας, διαγράφοντας και επισημαίνοντας τραγούδια της κάθε βιβλιοθήκης. Επιπλέον, με τη χρήση του τέρμιναλ μπορεί ο χρήστης αρκετά εύκολα να κατεβάσει τόρεντς της αρεσκείας του. Επιπροσθέτως, μπορεί πολύ εύκολα κάποιος χρήστης να διαχειριστεί μουσικά αλμπουμ καθώς επίσης και λίστες τραγουδιών. Τέλος, μέσω του τέρμιναλ ο χρήστης μπορεί να παρακολουθήσει ένα βίντεο από το youtube χώρις να χρειαστεί να το κατεβάσει στον υπολογιστή του.

### Βιβλιογραφία:
Google, Youtube, Man Unix, Github

# Συμμετοχικό εκπαιδευτικό υλικο:
# Twitter: [Προφίλ](https://twitter.com/p17chr1)

## 1ο tweet: [1o tweet](https://twitter.com/p17chr1/status/1193189008752496644)
## 2ο tweet: [2o tweet](https://twitter.com/p17chr1/status/1193190716308164609)
## 3ο tweet: [3o tweet](https://twitter.com/p17chr1/status/1193193040011255808)
## 4ο tweet: [4o tweet](https://twitter.com/p17chr1/status/1193205364864495618)
## 5ο tweet: [5o tweet](https://twitter.com/p17chr1/status/1193209204502417409)
## 6ο tweet: [6o tweet](https://twitter.com/p17chr1/status/1193216082670182400)
## 7ο tweet: [7o tweet](https://twitter.com/p17chr1/status/1193217986393497600)
## 8ο tweet: [8o tweet](https://twitter.com/p17chr1/status/1193220791766310914)
## 9ο tweet: [9o tweet](https://twitter.com/p17chr1/status/1193224890846973952)
## 10ο tweet: [10o tweet](https://twitter.com/p17chr1/status/1193227821646258183)



https://github.com/chris4dim/mm-Final_Report


---

Texnologia


---

Για να γίνει η εγκατάσταση του docker ακολούθησα τα παρακάτω βήματα κατά σειρά:

```

1)sudo apt-get update

2)sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
    
3)curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

4)sudo apt-key fingerprint 0EBFCD88

5)sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
6)sudo apt-get install docker-ce docker-ce-cli containerd.io
```
### Δημιουργία image Apache σε php με το Docker:
 Αρχικά δημιούργησα ένα αρχείο index.php σε ένα φάκελο που τον ονόμασα docker και χρησιμοποίησα το docker για να δημιουργήσω μία εικόνα "image" του Apache σε php χρησιμοποιώντας την παρακάτω εντολή:
 
```
 
 $ docker run -d -p 80:80 --name my-apache-php-app -v "$PWD":/var/www/html php:7.2-apache
 
```

Asciinema URL: [Docker](https://asciinema.org/a/MLQkYsRwftDMfEr65J3xUfudT)

### Με τη δημιουργία "εικόνας" Apache στο docker, μπορούμε να παμε στον browser Mozila Firefox και γράφοντας localhost εμφανίζεται ότι γράψαμε στο αρχείο index.php:

![Screenshot from 2020-03-02 22-22-39](https://user-images.githubusercontent.com/44117722/75714499-81e03c80-5cd4-11ea-988b-7d6d2700c3c3.png)







