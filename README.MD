# Geração de Batimentos Cardíacos com Imagens de Ultrassonografia

Este projeto utiliza imagens de ultrassonografia para gerar sons simulados de batimentos cardíacos. A frequência cardíaca é ajustada para ser condizente com diferentes estágios de desenvolvimento, como a frequência natural de um embrião de 10 semanas.

---

## 🔧 Funcionalidades
- Carrega imagens de ultrassonografia em 2D e processa os dados em escala de cinza.
- Converte intensidades dos pixels da imagem em frequências sonoras simulando batidas cardíacas.
- Gera som ajustado para frequências cardíacas naturais (exemplo: **110 a 160 BPM** para embriões).
- Aplica filtros passa-baixa para remover ruídos e suavizar o som.
- Adiciona pausas realistas entre as batidas para melhorar a qualidade.

---

## 📂 Estrutura do Projeto
- `ultrasound_to_heartbeat.py`: Código principal para processamento de imagem e geração de som.
- `frequencia_bebe.jpg`: Exemplo de imagem usada para simulação.
- `baby_natural.wav`: Som gerado com frequência cardíaca ajustada para embriões de 10 semanas.

---

## 💡 Pré-requisitos
Certifique-se de que você possui as seguintes bibliotecas instaladas:

```bash
pip install numpy
pip install soundfile
pip install scipy
pip install opencv-python
