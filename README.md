# Português


## 🎮✨ Genius no ESP32  

Um projeto divertido desenvolvido durante as aulas de **ESP32 na Bosch**, inspirado no clássico jogo da memória **Genius/Simon Says**.  
Nosso objetivo foi **replicar o jogo com LEDs, botões e buzzer**, trazendo sons e cores para a brincadeira.  

👉 Atualmente estamos evoluindo o projeto para integrar com um **site + API**, permitindo comunicação entre o jogo físico e uma interface web.  

---

### 🤯 Como funciona?

- O **ESP32** gera uma sequência aleatória de **LEDs coloridos**.  
- O jogador deve **memorizar e repetir a sequência** apertando os botões correspondentes.  
- Cada acerto aumenta o nível da rodada.  
- Se errar… 💥 **Game Over** com direito a sons e piscadas dramáticas.  

---

### ⚡ Demonstração física  

🔴🟢🟡🔵  
- **LEDs coloridos** para cada botão.  
- **Buzzer** para emitir sons diferentes para cada cor.  
- **Botões** mapeados com resistência interna `PULL_UP`.  

![ESP32](https://img.shields.io/badge/ESP32-MCU-blue?style=for-the-badge&logo=espressif)  
![Python](https://img.shields.io/badge/MicroPython-✔-green?style=for-the-badge&logo=python)  

---

### 🔧 Tecnologias usadas  

- [ESP32](https://www.espressif.com/en/products/socs/esp32)  
- **MicroPython**  
- **PWM + GPIO** (para LEDs e buzzer)  
- **Random** (para gerar sequências)  
- **API/Front-end (em desenvolvimento)**  

---

### 📂 Estrutura do código  

```
├── genius.py        # Código principal do jogo
├── README.md        # Este documento
└── (futuros arquivos do site/API)
```

---

### 🚀 Como rodar no seu ESP32

1. Instale o **MicroPython** no seu ESP32.  
2. Copie o arquivo `genius.py` para a placa (via `ampy`, `thonny`, `rshell`, etc).  
3. Conecte os LEDs, botões e buzzer nos pinos configurados:  

| Cor     | LED Pin | Botão Pin | Som (Hz) |
|---------|---------|-----------|----------|
| 🔴 Vermelho | 5       | 26        | 262      |
| 🟢 Verde    | 18      | 25        | 330      |
| 🟡 Amarelo  | 19      | 33        | 392      |
| 🔵 Azul     | 21      | 32        | 523      |

4. Rode o programa com:  

```python
import genius
```

---

### 🎶 Extras

- Cada cor tem seu **som único** 🎵.  
- Há uma **animação sonora/visual de derrota** 💀.  
- Em breve: **integração com site e API** 🌐.  

---

### 🧑‍💻 Autores

Projeto desenvolvido durante as aulas de **ESP32 na Bosch / Ctp-ETS**.  
Equipe: </br>
Angelina Henrique Chaves </br>
Juliano da Rocha Lesinski </br>
Nycolas Prado Seixa </br>

---

### 🌟 Status do projeto  

🚧 **Em andamento** – jogo físico pronto, agora estamos trabalhando na comunicação com API e front-end.  

---

### 💡 Ideias futuras

- Ranking de pontuação online.  
- Multiplayer conectado.  
- Versão web para jogar sem ESP32.  

---

# Inglês
</br>

## 🎮✨ Genius on ESP32  

A fun project developed during **ESP32 classes at Bosch**, inspired by the classic memory game **Genius/Simon Says**.  
Our goal was to **replicate the game with LEDs, buttons, and a buzzer**, bringing sounds and colors to the experience.  

👉 We are currently evolving the project to integrate with a **website + API**, allowing communication between the physical game and a web interface.  

---

### 🤯 How it works?

- The **ESP32** generates a random sequence of **colored LEDs**.  
- The player must **memorize and repeat the sequence** by pressing the corresponding buttons.  
- Each correct answer increases the level.  
- If you make a mistake… 💥 **Game Over** with dramatic sounds and flashing lights.  

---

### ⚡ Physical demo  

🔴🟢🟡🔵  
- **Colored LEDs** for each button.  
- **Buzzer** to play different tones for each color.  
- **Buttons** mapped with internal `PULL_UP` resistor.  

![ESP32](https://img.shields.io/badge/ESP32-MCU-blue?style=for-the-badge&logo=espressif)  
![Python](https://img.shields.io/badge/MicroPython-✔-green?style=for-the-badge&logo=python)  

---

### 🔧 Technologies used  

- [ESP32](https://www.espressif.com/en/products/socs/esp32)  
- **MicroPython**  
- **PWM + GPIO** (for LEDs and buzzer)  
- **Random** (to generate sequences)  
- **API/Front-end (under development)**  

---

### 📂 Project structure  

```
├── genius.py        # Main game code
├── README.md        # This document
└── (future website/API files)
```

---

### 🚀 How to run on your ESP32

1. Install **MicroPython** on your ESP32.  
2. Copy the `genius.py` file to the board (via `ampy`, `thonny`, `rshell`, etc).  
3. Connect the LEDs, buttons, and buzzer to the configured pins:  

| Color   | LED Pin | Button Pin | Sound (Hz) |
|---------|---------|------------|------------|
| 🔴 Red    | 5       | 26         | 262        |
| 🟢 Green  | 18      | 25         | 330        |
| 🟡 Yellow | 19      | 33         | 392        |
| 🔵 Blue   | 21      | 32         | 523        |

4. Run the program with:  

```python
import genius
```

---

### 🎶 Extras

- Each color has its **unique sound** 🎵.  
- There is a **visual/sound animation for defeat** 💀.  
- Coming soon: **website and API integration** 🌐.  

---

### 🧑‍💻 Authors

Project developed during **ESP32 classes at Bosch / Ctp-ETS**.  
Team: </br>
Angelina Henrique Chaves </br>
Juliano da Rocha Lesinski </br>
Nycolas Prado Seixa </br>

---

### 🌟 Project status  

🚧 **In progress** – physical game ready, now we are working on API and front-end communication.  

---

### 💡 Future ideas

- Online score ranking.  
- Connected multiplayer.  
- Web version to play without ESP32.  
