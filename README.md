# Zombie Necropolis
Il videogioco è stato sviluppato con Unreal Engine 5.
Nel file della release sono incluse esclusivamente le cartelle Content, Config e il file di progetto progettof.uproject. L’intero progetto non è stato caricato poiché troppo pesante; inoltre, sono state rimosse texture e file obsoleti per alleggerire il pacchetto.
Per la realizzazione dell’ambientazione è stata utilizzata una mappa scaricabile dal seguente link:
https://www.fab.com/listings/b3d214c2-50fa-4a0e-a780-bee56c1baf8f
Anche questa non è stata inclusa nei file della release in quanto troppo pesante.

 ## Come provare il videogioco:
- Aprire il progetto con Unreal Engine 5.
- Aprire una mappa qualsiasi.
- Inserire nella mappa il BP_EnemySpawner (cartella AI).
- Aggiungere un NavMeshBoundsVolume per permettere la generazione e il movimento degli zombie nella mappa.
- Modificare i valori di scala del NavMeshBoundsVolume in base alla grandezza della mappa utilizzata.
Potrebbero verificarsi problemi nella compilazione dell’ABP Body, poiché per la zombie walk era stato utilizzato uno scheletro troppo pesante, successivamente rimosso.
Per risolvere basta collegare il NewBlendSpace1D alla Source dello slot DefaultSlot nell’Animation Blueprint, gli zombie si muoveranno lentamente, poiché il valore della velocità è impostato sulla camminata tipica “zombie walk”.
