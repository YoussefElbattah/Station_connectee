# Station Connectée

## Description  
Le projet **Station Connectée** vise à concevoir une station environnementale basée sur des microcontrôleurs **STM32**.  
Il s’agit d’un système complet intégrant :

- Intégration et configuration de capteurs environnementaux et de vibrations sur carte STM32  
- Développement de l’affichage des données sur un écran **LCD 16×2**  
- Mise en place d’une **liaison LoRa** entre deux cartes STM32  
- Analyse et validation des protocoles **UART**, **SPI** et **I2C** à l’aide d’un **analyseur logique**

---

## Fonctionnalités  
- Acquisition de données environnementales (température, humidité, pression, etc.)
- Acquisition de données de vibrations  
- Affichage en temps réel sur un écran LCD 16×2  
- Transmission des données via **LoRa** entre deux cartes STM32  
- Validation des protocoles de communication (UART, SPI, I2C)  
- Analyse et visualisation des trames avec un analyseur logique  

---

## Matériel utilisé  
- Carte **STM32** (Nucleo L476RG)  
- Écran **LCD 16×2**
- X-NUCLEO-IKS02A1 
- Modules **LoRa E5**  
- Analyseur logique pour la validation des signaux  

---

## 🧩 Architecture du système  
1. Une **carte STM32** collecte les données des capteurs via I2C et/ou SPI.    
2. Une **deuxième carte STM32** reçoit ces données via la **liaison LoRa**.
3. Les valeurs reçues sont affichées sur un **écran LCD 16×2**.
4. Les protocoles UART, SPI et I2C sont analysés et validés à l’aide d’un analyseur logique.  

---

## 🚀 Installation et configuration  

### 🔧 Prérequis  
- **STM32CubeIDE** ou tout autre IDE compatible  
- Pilotes STM32 et bibliothèques **HAL** installées  
- Capteurs et modules LoRa correctement câblés  

### 🪜 Étapes  
1. **Cloner le dépôt :**
   ```bash
   git clone https://github.com/YoussefElbattah/Station_connectee.git
