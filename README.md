🎛️ MacroBoard Arduino – Teclado Programável com Macros, Sliders e Automação em Python

Este repositório contém um projeto de um MacroBoard programável utilizando Arduino Micro/Leonardo, keypad matricial, potenciômetros e scripts Python para automação no Windows.
O sistema permite envio de teclas, abertura de programas, navegação entre janelas e controle de volume via Python.

🎯 Objetivo do Projeto

Desenvolver um dispositivo compacto e funcional capaz de:

Enviar comandos de teclado (HID);

Executar macros personalizadas;

Controlar janelas (Alt+Tab, Delete, Ctrl+Z e outros);

Abrir programas automaticamente;

Enviar comandos para scripts Python;

Controlar volume do Windows com potenciômetro;

Ler sliders analógicos para uso externo (MIDI, automação, etc).

🧩 Componentes Utilizados

Arduino Micro ou Arduino Leonardo (compatível com HID)

Keypad matricial 3×4

4 potenciômetros (sliders)

1 potenciômetro exclusivo para volume (A1)

Jumpers para ligação

Protoboard ou PCB personalizada

🛠️ Como Funciona

O sistema lê as teclas do keypad e executa ações pré-programadas, como:

Abertura de Steam, Discord, WhatsApp, VSCode;

Alt+Tab para alternar janelas;

Delete e Ctrl+Z;

Execução de script Python para abrir o Valorant;

Controle de volume usando pycaw.

Os sliders conectados aos pinos A0–A3 enviam valores ao computador via serial (ou podem ser integrados ao Control Surface como MIDI).

📂 Estrutura do Repositório
├── main.ino                  # Código principal do Arduino
├── open_valorant.py          # Script Python para abrir o Valorant
├── volume_control.py         # Script Python para controle de volume
├── requirements.txt          # Dependências Python
├── /img                      # Fotos, diagramas e esquemas
└── README.md                 # Documentação principal

🚀 Como Executar o Projeto
1. Clone o repositório:
git clone https://github.com/seuusuario/seu-macroboard

2. Abra main.ino no Arduino IDE ou PlatformIO.
3. Instale as bibliotecas necessárias:

Keyboard.h

Keypad.h

Control_Surface

(Opcional) MIDIUSB

🧪 Testes e Validação

O MacroBoard foi testado em:

Controle de volume por potenciômetro A1;

Abertura de programas via Windows Search;

Execução de Valorant com argumentos via Python;

Resposta do keypad e antirruído;

Sliders analógicos retornando valores estáveis via Serial;

Teste de HID Keyboard funcionando no Windows.

👤 Autor

Matheus Henrique de Oliveira Sanches
Projeto pessoal / automação / eletrônica embarcada.
