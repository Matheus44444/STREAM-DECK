🎛️ MacroBoard Programável com Arduino + Python

Este repositório contém o desenvolvimento de um MacroBoard multifuncional, projetado para automação de tarefas, aumento de produtividade e controle rápido de funções no Windows.
O sistema combina a capacidade HID do Arduino Micro/Leonardo com automações avançadas em Python, criando uma ferramenta versátil, expansível e altamente personalizável.

📌 Objetivo do Projeto

O objetivo principal deste MacroBoard é fornecer uma interface de automação capaz de:

⌨️ Executar macros personalizadas via HID Keyboard

🖥️ Abrir softwares automaticamente (via Arduino ou Python)

🔄 Controlar janelas e funções do sistema (Alt+Tab, Delete, Ctrl+Z etc.)

🔊 Ajustar o volume do Windows através de um potenciômetro dedicado

🎚️ Enviar valores analógicos de sliders para uso externo (automação, efeitos, MIDI etc.)

🧩 Integrar funcionalidades avançadas usando scripts Python

🧩 Componentes Utilizados

Arduino Micro ou Arduino Leonardo (suporte HID nativo)

Teclado matricial 3×4

4 potenciômetros analógicos (sliders)

1 potenciômetro dedicado para o volume

Jumpers e protoboard ou PCB personalizada

Computador com Python 3.8+

🛠️ Como o Sistema Funciona
🔐 Arduino HID

O Arduino interpreta os comandos do teclado matricial e executa funções como:

Abrir Steam, Discord, WhatsApp, Visual Studio Code

Alternar janelas (Alt+Tab)

Executar comandos úteis (Delete, Ctrl+Z)

Acionar scripts Python externos

Controlar volume via leitura analógica (pino A1)

🎚️ Sliders Analógicos

Conectados aos pinos A0–A3, os sliders enviam valores continuamente para:

Controle de efeitos

Integração MIDI

Sistemas externos de automação

🚀 Como Executar o Projeto
1. Clonar o repositório
git clone https://github.com/seuusuario/seu-macroboard

2. Configurar o Arduino

Abra main.ino na Arduino IDE ou PlatformIO

Instale as bibliotecas:

Keyboard.h

Keypad.h

Control_Surface.h

Monte o circuito conforme o esquemático

Faça o upload para o Arduino Micro/Leonardo


🧪 Testes e Validação

O MacroBoard foi testado nas seguintes condições:

✔️ Abertura de programas via HID e scripts Python

✔️ Controle suave do volume via potenciômetro dedicado

✔️ Funcionamento estável do keypad matricial

✔️ Leitura consistente dos sliders analógicos

✔️ Execução automatizada do Valorant via chamada Python

✔️ Baixa latência e alta precisão nos comandos HID

📘 Scripts Disponíveis
Script	Função
open_valorant.py	Abre o Riot Client diretamente no Valorant
volume_control.py	Controla o volume do Windows via pycaw

Todos os scripts podem ser modificados conforme necessidade.

👤 Autor

Matheus Henrique de Oliveira Sanches
Projeto pessoal de automação, produtividade e sistemas embarcados.
