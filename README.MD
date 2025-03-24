# Geração de Batimentos Cardíacos com Imagens de Ultrassonografia

Projeto criado por um pai de primeira viagem, ansioso para escutar o coraçãozinho do bebê. Porém, como as primeiras ultrassonografias são feitas apenas em 2D, elas geram apenas imagens e não som. Por isso, decidi criar um código que me permita ouvir os batimentos cardíacos do meu bebê.

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

🚀 Como Usar

Prepare o ambiente: Instale as bibliotecas necessárias usando o comando acima.

Substitua a imagem: Substitua frequencia_bebe.jpg pela sua própria imagem de ultrassonografia, caso queira usar outra imagem.

Execute o código: Rode o script principal:

bash
python ultrasound_to_heartbeat.py
Ouça o som gerado: O arquivo de áudio será salvo como baby_natural.wav no diretório especificado.

📊 Configurações
Alterar a Faixa de Frequência Cardíaca
A frequência cardíaca padrão está definida entre 110 e 160 BPM. Você pode alterar isso modificando a linha:

python
frequency = np.interp(intensity, [0, 1], [110, 160])
Filtrar Som
Para suavizar ruídos ou ajustar o som, use o filtro passa-baixa incluído no código.

📄 Licença
Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais informações.

✨ Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar um pull request.

📞 Contato
Se tiver dúvidas, entre em contato pelo e-mail: seuemail@example.com


---

### Personalize Conforme Necessário
Sinta-se à vontade para ajustar seções como "Contato," adicionar imagens ou links relevantes, ou mesmo incluir exemplos de saída de som.

Se precisar de mais ajuda para formatar ou estruturar algo, estou à disposição! 😊
