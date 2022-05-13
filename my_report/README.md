# Lesson: Interaction Design

### First and Last Name: Ευαγγελία Δεσποτίδου
### University Registration Number: dpsd19030
### GitHub Personal Profile: [Evedes01](https://github.com/Evedes01)
### Augmented Reality Personal Repository: [Evedes01's AR Repository](https://github.com/Evedes01/Augmented-Reality)

# Introduction

# Summary


# 1st Deliverable
Αρχικά κατέβασα το ATOM στο οποίο έκανα επεξεργασία τον κώδικα. Μέσα από το Α-Frame School βρήκα τον κώδικα για την σφαίρα και τον κύλινδρο και τον εφάρμοσα στον κώδικά μου. Άλλαξα τις τιμές για τα μεγέθη, τις θέσεις και τα χρώματα των σχημάτων. Έπειτα, από τα link που δίνονται στην περιγραφή/ζητούμενα του Deliverable 1, βρήκα και αντέγραψα τον κώδικα για το χιόνι και τις φωνητικές εντολές. Τοποθέτησα τον κώδικα των φωνητικών εντολών μέσα στον κώδικα του χιονιού, ώστε να ενεργοποιείται/απενεργοποιείται με τις φωνητικές εντολές "start" και "stop". Καθ'όλη τη διάρκεια της διαδικασίας είχα ανοιχτό στον Google Chrome το παράθυρο του index, το οποίο έκανα συνεχώς refresh, ώστε να βλέπω στην πράξη τις αλλαγές που έκανα στον κώδικα και αν λειτουργεί σωστά. όλες τις εντολές τις δοκίμασα με των φωτογραφία "Hiro" από το κινητό.

# 2nd Deliverable
Για το 2ο μέρος αυτής της εργασίας (Deliverable 2) ξεκίνησα από το ζητούμενο του Custom marker με βάση το dpsd. Έφτιαξα το περιεχόμενο του marker σε ένα πρόγραμμα ζωγρφικής (Krita), και έπειτα το ανέβασα στο [AR.js Marker Training](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) για να φτιάξω τον marker.
<br>
![](pic1.PNG)
<br>
<br>
Στη συνέχεια πήγα στον κώδικα και έβαλα τον marker με την εντολή <a-marker> μέσα στο <a-scene>, έθεσα τον τύπο του marker και το έκανα λινκ με το url στο patt αρχείο, ώστε να διαβάζει η κάμερα τον marker. Μετά έβαλα το κείμενο (το οποίο και μορφοποίησα με τις κατάλληλες εντολές που βρήκα [εδώ](https://aframe.io/docs/1.3.0/components/text.html)) και τη φωτογραφία (επίσης μορφοποιώντας με τις κατάλληλες εντολές. Τέλος τοποθέτησα και τα δύο στο κέντρο του marker με μια εντολή <a-entity>.
<br>
![](pic2.PNG)
<br>
Δυστυχώς, στην αρχή δεν δούλεψε, καθώς αντιμετώπισα πρόβλημα με το CORS policy, οπότε δοκίμασα να αντικαταστήσω τον custom marker με τον hiro marker, όπου, αυτή τη φορά εμφανίστηκαν στην κάμερα μόνο τα γράμματα και ένα άσπρο τετράγωνο αντί της φωτογραφίας. Τελίκά, έλυσα το πρόβλημα χρησιμοποιώντας έναν local server, τον οποίο έκανα set-up με την βοήθεια της pyhton, και αφού βεβαιώθηκα ότι τα αρχεία δουλεύουν με το hiro marker ξανά έβαλα τον custom dpsd marker. Και έχει το εξής οπτικό αποτέλεσμα 
 ![](cam1.png)
 <br>
Για τους marker του υδρογόνου και του οξυγόνου ακολούθησα την ίδια διαδικασία με τον custom. Μέσα στους marker έχω καταχωρήσει τις αντίστοιχες οικόνες των στοιχείων και τα αντίστοιχα 3D μοντέλα σε glb format. Τα μοντέλα και το animation τα έφτιαξα στο Blender σύμφωνα με το [αυτό](https://www.youtube.com/watch?v=HfnMmN1nYYQ&t=647s&ab_channel=DerekElliott) το βίντεο.
<br> Παρακάτω είναι ο κώδικας για τα στοιχεία.
<br> 
![](pic3.PNG)
![](pic4.PNG)
<br>
 <br>
Για να λειτουργήσει το animation των 3D μοντέλων με την εντολή *animation-mixer* εισήγαγα το εξής [script](https://cdn.jsdelivr.net/gh/donmccurdy/aframe-extras@v6.1.1/dist/aframe-extras.min.js) στην αρχή του κώδικα και χρησιμοποιήσα τις εντολές που φαίνονται παρακάτω για να προσαρμώσω το animation (για αυτά τα βήματα συμβουλεύτηκα αυτήν τη [σελίδα](https://stackoverflow.com/questions/70735151/a-frame-pause-play-animation-mixer) και την σελίδα του A-Frame για τα animation 3D μοντέλων:
 <br>
 ![](pic5.PNG)
 <br>
<br>
 Τέλος, προγραμμάτησα τον αλγόριθμο της απόστασης μεταξύ των markers με JavaScript σύμφωνα με αυτά τα links: [link1](https://stackoverflow.com/questions/61239107/how-to-get-marker-position-x-y-ar-js) και [link2](https://aframe.io/docs/0.8.0/introduction/writing-a-component.html). Επίσης, προσέθεσα το 3D μοντέλο του νερού στον marker του οξυγόνου, όπως και την κάρτα για το νερό, την οποία έφτιαξα στο Krita.
 <br>
 ![](pic6.PNG)
 ![](pic7.PNG)
 <br>
 <br>Στα δύο προαναφερόμενα εφάρμωσα την εντολή *visible="false"*, ![](pic8.PNG) ώστε να είναι κρυφά στην αρχή και να εμφανίζονται μόνο όταν πληρείται η προϋπόθεση της απόστασης, που ορίζεται στον κώδικα JavaScript, ο οποίος είναι τοποθετημένος στο *body* πάνω από το *a-scene*.
 <br>
 <br>
 Το τελικό αποτέλεμα είναι το εξής:
 <br>
 ![](cam2.png)
 ![](cam3.png)
# 3rd Deliverable 


# Conclusions


# Sources
