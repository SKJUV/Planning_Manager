# 📅 Planning Manager — Module de Gestion d'Emplois du Temps

[![Java](https://img.shields.io/badge/Java-17-ED8B00?logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Maven](https://img.shields.io/badge/Build-Maven-C71A36?logo=apache-maven&logoColor=white)](https://maven.apache.org/)
[![GUI](https://img.shields.io/badge/UI-Java%20Swing-5382A1)](https://docs.oracle.com/javase/tutorial/uiswing/)
[![Tests](https://img.shields.io/badge/Tests-JUnit%204-25A162?logo=junit5&logoColor=white)](https://junit.org/)

Application de gestion, structuration et visualisation matricielle d'emplois du temps universitaires et académiques développée en **Java 17** avec interface graphique **Java Swing**.

---

## 🎯 Objectifs & Fonctionnalités

- 📊 **Visualisation Matricielle Dynamique** : Affichage hebdomadaire des créneaux horaires, salles et matières sous forme de tableau interactif `JTable`.
- ⚡ **Sécurité de Rendu UI** : Exécution thread-safe du cycle graphique sur l'Event Dispatch Thread (EDT) via `SwingUtilities.invokeLater`.
- 🏛️ **Architecture Modulaire** : Modèles de données découplés (`Planning.java`), séparation entre la vue Swing et les schémas SQL relationnels.
- 🧪 **Intégration Continue & Tests** : Suite de tests unitaires JUnit orchestrée via le cycle de vie Apache Maven.

---

## 🏗️ Structure du Projet

```text
Planning_Manager/
├── pom.xml                               # Configuration Maven (Java 17, JUnit 4)
├── src/
│   ├── main/
│   │   ├── java/com/g9/
│   │   │   ├── Main.java                 # Fenêtre principale et interface Swing
│   │   │   └── model/
│   │   │       └── Planning.java         # Modèle objet des plannings et créneaux
│   │   └── resources/
│   │       └── schema.sql                # Schéma relationnel de persistance
│   └── test/
│       └── java/com/g9/
│           └── AppTest.java              # Tests unitaires
```

---

## 🚀 Démarrage Rapide

### Prérequis
- **Java JDK 17** ou supérieur
- **Apache Maven 3.8+**

### Compilation & Lancement
```bash
# 1. Cloner le dépôt
git clone https://github.com/SKJUV/Planning_Manager.git
cd Planning_Manager

# 2. Compiler avec Maven
mvn clean compile

# 3. Lancer les tests unitaires
mvn test

# 4. Exécuter l'application
mvn exec:java -Dexec.mainClass="com.g9.Main"
```

---

## 📄 Licence & Contribution
Projet académique collaboratif conçu dans le cadre des travaux pratiques en Génie Logiciel & Programmation Orientée Objet (Université de Yaoundé I).
