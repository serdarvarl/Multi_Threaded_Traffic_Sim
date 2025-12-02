[🇺🇸 English](#-traffic-simulation-system-java-swing) | [🇫🇷 Français](#-système-de-simulation-de-trafic-java-swing)

---

# 🚦 Traffic Simulation System (Java Swing)

A multi-threaded graphical simulation of traffic flow at an intersection, built with **Java Swing**. This project models the interaction between vehicles, pedestrians, and traffic lights using concurrent programming concepts.

![Traffic Simulation Screenshot](screenshot.png)

## 📋 Overview
This application simulates a real-time traffic environment where:
* **Vehicles** (Blue rectangles) move along the X-axis.
* **Pedestrians** (Orange circles) cross along the Y-axis.
* **Traffic Lights** control the flow, switching states automatically.

The simulation logic ensures safety: Vehicles stop at red lights, and pedestrians only cross when it is safe.

## ⚙️ Technical Features
* **Concurrency & Multithreading:** Utilizes `ExecutorService` to manage separate threads for each vehicle, pedestrian, and traffic light, ensuring smooth concurrent execution.
* **Custom Map Parsing:** The environment layout (roads, sidewalks, crosswalks) is dynamically loaded from a `plan.csv` file into a 2D grid.
* **Real-time Rendering:** A Swing `Timer` refreshes the UI every 16ms (~60 FPS) for smooth animation.
* **Object-Oriented Design:** Modular structure with separate classes for `Vehicules`, `Pietons`, and `Feu` (Traffic Lights).

## 🛠️ Built With
* **Language:** Java
* **GUI Framework:** Java Swing (`JPanel`, `Graphics`)
* **Data Source:** CSV (Comma Separated Values)

## 👥 Credits & Team
This project was developed as a collaborative effort:
* **Serdar VAROL:** Simulation logic, Thread management (`SimulationPanel`), and integration.
* **Hazem IBNMTAR:** Traffic Light (`Feu`) logic and implementation.
* **Lydia MOUTCHACHOU:** Map design and CSV data structure (`plan.csv`).

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone "take true repo from github"
    ```
2.  Open the project in your favorite IDE (IntelliJ IDEA, Eclipse, or VS Code).
3.  Ensure `plan.csv` is in the root directory.
4.  Run the `Main` class.

---

# 🚦 Système de Simulation de Trafic (Java Swing)

Une simulation graphique multi-thread du flux de trafic à un carrefour, construite avec **Java Swing**. Ce projet modélise l'interaction entre les véhicules, les piétons et les feux de circulation en utilisant des concepts de programmation concurrente.

![Capture d'écran de la simulation](screenshot.png)

## 📋 Vue d'ensemble
Cette application simule un environnement de trafic en temps réel où :
* Les **Véhicules** (rectangles bleus) se déplacent le long de l'axe X.
* Les **Piétons** (cercles oranges) traversent le long de l'axe Y.
* Les **Feux de circulation** contrôlent le flux et changent d'état automatiquement.

La logique de simulation assure la sécurité : les véhicules s'arrêtent aux feux rouges, et les piétons ne traversent que lorsque c'est sûr.

## ⚙️ Fonctionnalités Techniques
* **Concurrence & Multithreading :** Utilise `ExecutorService` pour gérer des threads séparés pour chaque véhicule, piéton et feu, assurant une exécution concurrente fluide.
* **Analyse de Carte Personnalisée :** La disposition de l'environnement (routes, trottoirs, passages piétons) est chargée dynamiquement depuis un fichier `plan.csv` dans une grille 2D.
* **Rendu en Temps Réel :** Un `Timer` Swing rafraîchit l'interface toutes les 16ms (~60 FPS) pour une animation fluide.
* **Conception Orientée Objet :** Structure modulaire avec des classes séparées pour `Vehicules`, `Pietons`, et `Feu`.

## 🛠️ Technologies Utilisées
* **Langage :** Java
* **Interface Graphique (GUI) :** Java Swing (`JPanel`, `Graphics`)
* **Source de données :** CSV (Comma Separated Values)

## 👥 Crédits & Équipe
Ce projet a été développé dans le cadre d'un effort collaboratif :
* **Serdar VAROL :** Logique de simulation, gestion des Threads (`SimulationPanel`) et intégration.
* **Hazem IBNMTAR :** Logique et implémentation des feux de circulation (`Feu`).
* **Lydia MOUTCHACHOU :** Conception de la carte et structure des données CSV (`plan.csv`).

## 🚀 Installation et Exécution
1.  Cloner le dépôt :
    ```bash
    git clone "prendre correct repo depuis github car il a ete renommer"
    ```
2.  Ouvrir le projet dans votre IDE préféré (IntelliJ IDEA, Eclipse, ou VS Code).
3.  S'assurer que le fichier `plan.csv` se trouve dans le répertoire racine.
4.  Lancer la classe `Main`.