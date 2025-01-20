### Partie 1 : Gestion des Utilisateurs 

Q 2.1.1

![VirtualBox_Checkpoint3-SRVLX01_17_01_2025_11_50_31](https://github.com/user-attachments/assets/8824e434-87ce-451f-b3bd-bbe29835f600)

Q 2.1.2 
> 1. Mettre un mot de passe à 12 caractères et une lettre majuscule,des caractères spécieaux et des chiffres. 
> 2. Authentification par connexion SSH uniquement par une clé privé et une clé public 
> 3. Enlever l'authenfication par mot de passe via la connexion SSH 


### Partie 2 : Configuration SSH 
Q 2.2.1 et 2.2.3 


![VirtualBox_Checkpoint3-SRVLX01_17_01_2025_12_03_05](https://github.com/user-attachments/assets/a97160fc-a9be-4f1b-a833-ee97371e309a)

![VirtualBox_Checkpoint3-SRVLX01_17_01_2025_12_03_35](https://github.com/user-attachments/assets/9b2cb7de-f9b9-49b1-8029-2bba6b4ee2d3)

Q 2.2.3

![VirtualBox_Checkpoint3-SRVLX01_19_01_2025_19_54_36](https://github.com/user-attachments/assets/e5794e9e-cca4-4429-8284-9faa50887415)


![VirtualBox_Checkpoint3-SRVLX01_19_01_2025_20_11_23](https://github.com/user-attachments/assets/ddc926fa-eefe-452a-915c-c9528dfa9aa0)


![VirtualBox_Checkpoint3-SRVLX01_17_01_2025_12_18_23](https://github.com/user-attachments/assets/4507f25c-8ae1-4689-ac79-476a1a10935b)

### Partie 3 : Analyse du stockage 

Q 2.3.1 
> 1. Les systèmes de fichiers montés sont : udev,tmpfs,dev/mdp01,dev/mapper/cp3--vg-root

Q 2.3.2
> 2. Ils utilisent le RAID et LVM 

Q 2.3.3 

![VirtualBox_Checkpoint3-SRVLX01_20_01_2025_10_33_00](https://github.com/user-attachments/assets/d11ad00e-926f-4123-be4f-5b7ad5d90791)

Q 2.3.4 

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_01_05](https://github.com/user-attachments/assets/dce7cbcd-50f8-4fba-80c1-29fafad33721)

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_07_58](https://github.com/user-attachments/assets/756c8418-72a6-415f-9bfd-0fb9258ff421)

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_08_23](https://github.com/user-attachments/assets/df76bf7f-bdf9-4fc5-9e83-67b4758e1001)

Q 2.3.5 

> 1. Il reste 5Gio sur le volume disque 

### Partie 4 : Sauvegardes 

Q 2.4.1
> bareos-dir (Director) :

    Rôle : Le Director est le composant central de Bareos. Il orchestre les opérations de sauvegarde, de restauration et de vérification.
    Responsabilités :
        Planifier les tâches de sauvegarde en fonction des configurations définies.
        Gérer les communications avec les autres composants (Storage Daemon et File Daemon).
        Maintenir une base de données pour stocker les métadonnées des sauvegardes (fichiers sauvegardés, dates, etc.).

> bareos-sd (Storage Daemon) :

    Rôle : Le Storage Daemon est responsable de la gestion des supports de stockage où les données sauvegardées sont écrites.
    Responsabilités :
        Recevoir les données à sauvegarder du File Daemon via le Director.
        Écrire les données sur les supports de stockage configurés (disques, bandes magnétiques, etc.).
        Fournir les données demandées lors des restaurations.

> bareos-fd (File Daemon) :

    Rôle : Le File Daemon est installé sur les machines à sauvegarder (clients). Il est responsable de fournir les fichiers à sauvegarder.
    Responsabilités :
        Préparer et transmettre les données des fichiers/dossiers spécifiés au Storage Daemon via le Director.
        Participer à la restauration en récupérant les fichiers depuis le Storage Daemon.

### Partie 5 : FIltrage et analyse réseau 

Q 2.5.1 

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_29_23](https://github.com/user-attachments/assets/f7989833-14c8-48c7-8741-7a9539388e7c)

Q 2.5.2 
> Connexion par SSH sur le port 22 

Q 2.5.3 
> policy drop 
> ct state invalid drop 

Q 2.5.4 

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_50_16](https://github.com/user-attachments/assets/cddb634c-5e4b-4ccd-9878-4ee945cc3521)

### Partie 6 : Analyse de logs 

![VirtualBox_Checkpoint3-SRVLX01 1_20_01_2025_22_57_13](https://github.com/user-attachments/assets/23d3deb1-7c05-4346-abd4-3eee36f85a45)


