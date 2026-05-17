# LAB19Dev
# LAB 19 : Room, MVVM, Repository, ViewModel, LiveData et RecyclerView

## 📚 Description

Ce laboratoire consiste à développer une application Android en Java utilisant l’architecture MVVM avec Room Database afin de gérer des notes locales.

L’application permet :

* d’ajouter des notes
* d’afficher les notes dans un RecyclerView
* de supprimer toutes les notes
* de sauvegarder les données localement avec Room

---

# 🛠️ Technologies utilisées

* Java
* Android Studio
* Room Database
* MVVM
* LiveData
* ViewModel
* RecyclerView
* Repository Pattern

---

# 📁 Structure du projet

```text
com.example.roommvvmdemo
│
├── data
│   ├── local
│   │   ├── Note.java
│   │   ├── NoteDao.java
│   │   └── NoteDatabase.java
│   │
│   └── NoteRepository.java
│
├── ui
│   ├── MainActivity.java
│   └── NoteAdapter.java
│
└── viewmodel
    └── NoteViewModel.java
```

---

# ⚙️ Dépendances utilisées

```gradle
val roomVersion = "2.8.4"
val lifecycleVersion = "2.9.3"

implementation("androidx.room:room-runtime:$roomVersion")
annotationProcessor("androidx.room:room-compiler:$roomVersion")
implementation("androidx.room:room-ktx:$roomVersion")

implementation("androidx.lifecycle:lifecycle-viewmodel:$lifecycleVersion")
implementation("androidx.lifecycle:lifecycle-livedata:$lifecycleVersion")

implementation("androidx.recyclerview:recyclerview:1.4.0")
implementation("androidx.cardview:cardview:1.0.0")
```

---

# 🧠 Architecture MVVM

```text
MainActivity
      ↓
NoteViewModel
      ↓
NoteRepository
      ↓
NoteDao
      ↓
Room Database
```

---

# 📱 Fonctionnalités réalisées

✅ Ajout d’une note

✅ Affichage des notes avec RecyclerView

✅ Suppression de toutes les notes

✅ Sauvegarde locale avec Room Database

✅ Utilisation de LiveData et ViewModel

✅ Architecture MVVM complète

---

# 📸 Résultat final

<img width="429" height="766" alt="37" src="https://github.com/user-attachments/assets/1811acc2-f620-4301-949e-f3bf6d6500aa" />


---

# 🚀 Exécution du projet

1. Cloner le projet

```bash
git clone <url-du-repository>
```

2. Ouvrir le projet dans Android Studio

3. Synchroniser Gradle

4. Lancer l’émulateur Android

5. Exécuter l’application

---

# ✅ Conclusion

Ce laboratoire a permis de comprendre l’architecture MVVM sous Android et l’intégration de Room Database pour la persistance locale des données.

L’utilisation de LiveData, ViewModel et Repository améliore la maintenance, la lisibilité et l’organisation du projet Android.
