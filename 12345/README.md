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

### Για να γίνει η εγκατάσταση του docker ακολούθησα τα παρακάτω βήματα κατά σειρά:

```

1) $ sudo apt-get update

2) $ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
    
3) $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

4) $ sudo apt-key fingerprint 0EBFCD88

5) $ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
6) $ sudo apt-get install docker-ce docker-ce-cli containerd.io
```
### Δημιουργία image Apache σε php με το Docker:
 Αρχικά δημιούργησα ένα αρχείο index.php σε ένα φάκελο που τον ονόμασα docker και χρησιμοποίησα το docker για να δημιουργήσω μία εικόνα "image" του Apache σε php χρησιμοποιώντας την παρακάτω εντολή:
 
```
 
 $ docker run -d -p 80:80 --name my-apache-php-app -v "$PWD":/var/www/html php:7.2-apache
 
```

### Asciinema URL: [asciinema](https://asciinema.org/a/2WotEN86jJDNILA4YkEDPTSC6)

### Με τη δημιουργία "εικόνας" Apache στο docker, μπορούμε να παμε στον browser Mozila Firefox και γράφοντας localhost εμφανίζεται ότι γράψαμε στο αρχείο index.php:

![Screenshot from 2020-03-02 22-22-39](https://user-images.githubusercontent.com/44117722/75714499-81e03c80-5cd4-11ea-988b-7d6d2700c3c3.png)

### Κάποιες χρήσιμες εντολές είναι οι παρακάτω:

Container που τρέχει.
```
 $ docker ps
```
Containers που τρέχουν ή είναι ανενεργά.
```
 $ docker ps -a
```
Τερματίζω ένα conatainer.
```
 $ docker stop "id"
```
Σβήνω ένα container αφού πρώτα το σταματήσω με την παραπάνω εντολή.
```
 $ docker rm "id"
```
Βλέπω όλα τα "images"
```
 $ docker images
```
Σβήνω ένα "image".
```
 $ docker rmi "id"
```



### References

[docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
[dockerhub](https://hub.docker.com/_/php)

---
### Για να γίνει η εγκατάσταση του Ntfy έγραψα την παρακάτω εντολή:

```
 $ sudo pip install ntfy
```
Το επόμενο βήμα ήταν να ενεργοποιήσω τα μηνύματα και να στέλνονται μετά την ολοκλήρωση της κάθε εργασίας. Αυτό πραγματοποιήθηκε γράφωντας την παρακάτω εντολή στο .bashrc με nano .bashrc:

```
 eval "$(ntfy shell-integration)"
```
Για να πραγματοποιήσω την εργασία κατέβασα ένα βίντεο από το youtube με τη χρήση του youtube-dl όπως φαίνεται στο παρακάτω βίντεο που έφτιαξα. Με την ολοκλήρωση του κατεβάσματος του βίντεο στάλθηκε μήνυμα ότι ολοκληρώθηκε η διεργασία του κατεβάσματος όπως φαίνεται παρακάτω.

![ntfy3](https://user-images.githubusercontent.com/44117722/76169046-5ef2d400-617d-11ea-95f7-e25dab899b56.png)

### Asciinema URL: [asciinema](https://asciinema.org/a/yrLNEWHwtuYB7RuSYbHD79F6Q)

### Όταν κατέβηκε το αρχείο βίντεο εμφανίστηκε το μήνυμα πάνω από το τέρμιναλ.
![Screenshot from 2020-03-08 19-50-25](https://user-images.githubusercontent.com/44117722/76168422-6c598f80-6178-11ea-92da-c9378161fe24.png)

### References

[ntfy](https://github.com/dschep/ntfy)

---


### Για να γίνει η εγκατάσταση του OpenSSH έγραψα αρχικά την παρακάτω εντολή:
```
 $ sudo apt-get install openssh-server
```
Για να γίνει η επιβεβαίωση ότι η εγκατάσταση ήταν επιτυχής έγραψα την παρακάτω εντολή, όπου είδα στο τέρμιναλ το μήμυμα Active: active (running):

```
 $ sudo systemctl status ssh
```
Το επόμενο βήμα ήταν να ενεργοποιήσω το "firewall" του συστήματος με την παρακάτω εντολή:
```
 $ sudo ufw allow ssh
```
Τέλος, για την σύνδεση δύο συστημάτων χρησιμοποίησα την παρακάτω εντολή:
```
 $ ssh username@ip_address
```
Όπου το username είναι το όνομα του συστήματος και ip_address είναι η διεύθυνση και βρίσκονται από την παρακάτω εντολή:
```
 $ ip a
```

Στη συγκεκριμένη εργασία χρησιμοποίησα ένα λάπτοπ με λειτουργικό Ubuntu 16.04 και ένα Raspberry pi 4 με λειτουργικό Raspbian. Αφού πρώτα έκανα όλη την παραπάνω διαδικασία σχετικά με την εγκατάσταση χρησιμοποίησα το username του Raspberry pi 4 και την διευθυνση ip, όπως φαίνεται παρακάτω.


![myscreen](https://user-images.githubusercontent.com/44117722/76658074-f2f8dd00-657b-11ea-9328-5248f4648c49.png)

Στη συνέχεια χρησιμοποίησα την παρακάτω εντολή για τη σύνδεση των δύο συστημάτων:
```
 $ ssh pi@192.168.1.21
```
Αφού λοιπόν έγινε η σύνδεση των δύο συστημάτων, από το τέρμιναλ του λειτουργικού συστήματος Ubuntu εκτέλεσα το αρχείο cv με nano cv, το οποίο ήταν αποθηκευμένο στο Raspberry pi 4. Όλη η διαδικασία περιγράφεται παρακάτω στο βίντεο:

### Asciinema URL: [asciinema](https://asciinema.org/a/WjQ1cvKtJcGpUtuwJ34ZUYIes)

### Το αρχείο cv κατά την εκτελέση του απο το απομακρυσμένο σύστημα Ubuntu.

![Screenshot from 2020-03-13 21-47-12](https://user-images.githubusercontent.com/44117722/76658933-d8bffe80-657d-11ea-9993-11e9de8f5052.png)

### References

[openSSh](https://linuxize.com/post/how-to-enable-ssh-on-ubuntu-18-04/)

---
Για να γίνει η εγκατάσταση του hyperfine έγραψα τις παρακάτω εντολές στο τέρμιναλ:

```
 1) $ wget https://github.com/sharkdp/hyperfine/releases/download/v1.9.0/hyperfine_1.9.0_amd64.deb
 
 2) $ sudo dpkg -i hyperfine_1.9.0_amd64.deb
```

Για την εκπόνηση της εργασίας αυτής χρησιμοποιήθηκαν δύο python scripts, ώστε να γίνει παρακολούθηση των αρχείων αυτών κατά την εκτέλεσή τους. Πιο συγκεκριμένα, χρησιμοποιήθηκαν τα αρχεία example1.py και example2.py, όπου με την χρήση της παρακάτω εντολής βγήκαν κάποια αποτλέσμαατα όσον αφορά τον χρόνο εκτέλεσής τους (ελάχιστο, μέγιστο, μέσο χρόνο και μαζί με την τυπική απόκλιση).

```
 $ hyperfine 'pyhton3 example1.py' 'python3 example2.py'
```

### Asciinema URL: [asciinema](https://asciinema.org/a/Hlyjysq7KhFegTIvReVB16Fu9)

Ακόμη, υπάρχει η δυνατότητα τα αποτελέσματα να εξαχθούν σε εξωτερικό αρχείο, για παράδειγμα σε αρχείο output.csv και αυτό επιτεύχθηκε με την παρακάτω εντολή:

```
 $ hyperfine --export-csv output 'pyhton3 example1.py' 'python3 example2.py'
```
### Τα αποτελέσματα στο αρχείο output.csv
![hyperfine](https://user-images.githubusercontent.com/44117722/76889676-af111b00-688e-11ea-91ba-aab67618e128.png)

### References

[Hyperfine](https://github.com/sharkdp/hyperfine)

---

Για να γίνει η διεκπεραίωση της εργασίας αυτής έκανα τη χρήση 5 διαφορετικών τέρμιναλς (guake, konsole, tilda, yuakake και terminology) και έγινε η εγκατάσταση αυτών με τις παρακάτω εντολες:

```
 $ sudo apt-get -f install guake
 $ sudo apt-get -f install konsole
 $ sudo apt-get -f install tilda
 $ sudo apt-get -f install yuakake
 $ sudo apt-get -f install terminology
```
Για την επίδειξη του κάθε τέρμιναλ χρησιμοποίησα απλές εντολές, οποίες περιγράφονται στο αντίστοιχο βίντεο του aasciinema, δημιουργώντας κάθε φορά ένα φάκελο με το όνομα του κάθε τέρμιναλ και μέσα σε αυτόν ένα αρχείο python με όνομα hello.py και με έξοδο κατα την εκτέλεσή του "hello world!!!". Κατά την καταγραφή της διαδικασίας του εκάστοτε τέρμιναλ χρησιμοποίηθηκε το asciinema και ένα αντίστοιχο στιγμιότυπο "screenshot" για την επίδειξη του αποτελέσματος, καθώς στα βίντεο δεν καταγράφονται τα χρώματα και άλλα χαρακτηριστικά του κάθε τέρμιναλ.

### guake: είναι ένα τέρμιναλ, όπου ο χρήστης το μετακινεί στο πάνω ή στο κάτω μέρος της οθόνης, πατώντας το πλήκτρο F12 και είναι γραμένο σε python. Τέλος, ο χρήστης μπρεί να αλλάξει την εμφάνισή του καθώς επίσης και να αλλάξει και τα διάφορα πλήκτρα με βάση τις ανάγκες του.

### Asciinema URL: [guake](https://asciinema.org/a/gzz8Ei9dT3bhcdFgyLtzcKjJL)

### Εικόνα του τέρμιναλ "guake".

![guake](https://user-images.githubusercontent.com/44117722/77182803-02c17580-6ad6-11ea-91d3-7c7b98f7de32.png)

### konsole

### Asciinema URL: [konsole](https://asciinema.org/a/pXYzb2EAjgaVDGJlWKxVMTSlM)

### Εικόνα του τέρμιναλ "konsole".

![konsole](https://user-images.githubusercontent.com/44117722/77183180-9abf5f00-6ad6-11ea-81ae-f49038457c1e.png)

### tilda: είναι ένα τέρμιναλ, που δεν καταλαμβάνει ολόκληρη την οθόνη, αλλά έχει το χαρακτηριστικό να μετακινείς το τέρμιναλ στο πάνω ή στο κάτω μέρος της οθόνης, χρησιμοποιώντας το F1 πλήκτρο. Επίσης, υπάρχει το χαρακτηριστικό ότι ο χρήστης μπορεί να αλλάξει την εμφάνισή του, αλλάζοντας τον φόντο του τέρμιναλ. Τέλος, υπάρχει η δυνατότητα αλλαγής πλήκτρων με βάση τις ανάγκες μας.

### Asciinema URL: [tilda](https://asciinema.org/a/uvMgNoIrHYh0yVr9nNxMCmAid)

### Εικόνα του τέρμιναλ "tilda".
![tilda](https://user-images.githubusercontent.com/44117722/77183469-09042180-6ad7-11ea-96c0-6284ef2dced0.png)


### yakuake: είναι ένα τέρμιναλ, το οποίο μετακινείται στο πάνω και στο κάτω μέρος της οθόνης, πατώντας το πλήκτρο F12. Αποτελεί ένα ελαφρύ τέρμιναλ με πολλά χαρακτηριστικά και γρήγορο ευρετήριο.

### Asciinema URL: [yakuake](https://asciinema.org/a/Aed4S6XajE9Kpk4JY3N7JCLyu)
### Εικόνα του τέρμιναλ "yakuake".
![yakuake](https://user-images.githubusercontent.com/44117722/77183870-a3fcfb80-6ad7-11ea-8182-59f7714f9e1d.png)


### terminology
### Asciinema URL: [terminology](https://asciinema.org/a/FmQ6j8i9HLt1avNbnj608mFON)
### Εικόνα του τέρμιναλ "terminology".
![terminology](https://user-images.githubusercontent.com/44117722/77184148-0d7d0a00-6ad8-11ea-808d-c4abc4beb09b.png)

### Στη συγκεκριμένη εργασία έγινε η εγκατάσταση και η χρήση του shell "fish" και η επίδειξη του με βίντεο μέσω του asciinema. Χρησιμοποίηθηκε για την δημιουργία ενός φακέλου με το όνομα "fish" και η δημιουργία σε αυτόν ένα αρχείο hello.py, όπου δίνει το αποτέλεσμα "hello world!!!". Για την εγκατλασταση χρησιμοποιήθηκαν κατά σειρα οι παρακάτω εντολές:
```
 1) $ sudo apt-add-repository ppa:fish-shell/release-3
 2) $ sudo apt-get update
 3) $ sudo apt-get install fish
```
### Asciinema URL: [fish](https://asciinema.org/a/nlhsWjVWQEb320ttdMNeLMPv3)

### References

[fishshell](https://launchpad.net/~fish-shell/+archive/ubuntu/release-3)
[terminals](https://linuxhint.com/best_terminal_aternatives_ubuntu/)

---

 asciinema URL: [Mysite](https://asciinema.org/a/SjSHKU6FzCrbk3xICiP1y7SGj)



