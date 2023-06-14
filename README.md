# Reconhecimento Facial

Projeto final da matéria Tópicos Avançados em Informática I do curso Bacharelado em Ciências e Tecnologia da Universidade Federal do Rio Grande do Norte (UFRN)

Professor:
  - Orivaldo Vieira de Santana Junior

Alunos:
  - Maria Clara Moura de Freitas
  - Yuri Ferreira Borges
  
- Código: https://colab.research.google.com/drive/1Zxn99J_s-ciUkrdRKu-BQuxIX7UKVXsE
- Referencia: 
https://jakevdp.github.io/PythonDataScienceHandbook/05.09-principal-component-analysis.html
https://patotricks15.medium.com/detec%C3%A7%C3%A3o-de-faces-com-python-opencv-modelo-haar-cascade-485bc1bcb368
- Dataset faces: http://vis-www.cs.umass.edu/lfw/#download

# Etapas:

## Configuração do ESP-CAM
O objetivo deste projeto é realizar o reconhecimento facial utilizando um ESP-CAM, Python e um servidor. O ESP-CAM é conectado a um microcontrolador ESP32 e é necessário ter a biblioteca adequada para acessar a câmera. Além disso, a configuração da conexão Wi-Fi no ESP-CAM é fundamental para que ele possa se conectar ao servidor.

## Captura da imagem
Para capturar a imagem, é necessário utilizar a biblioteca apropriada no microcontrolador que permita acessar a câmera do ESP-CAM. Com a biblioteca configurada, é possível capturar a imagem e salvá-la no microcontrolador para uso posterior.

## Envio da imagem para o servidor
A imagem capturada precisa ser enviada para o servidor para processamento. Isso é feito estabelecendo uma conexão entre o ESP-CAM e o servidor, utilizando o protocolo HTTP ou MQTT. Através dessa conexão, a imagem capturada é enviada ao servidor para que possa ser processada.

## Processamento da imagem no servidor
No servidor, é utilizado o Python para receber a imagem enviada pelo ESP-CAM. Para realizar o reconhecimento facial, bibliotecas como OpenCV, dlib ou TensorFlow são empregadas para processar a imagem. É necessário treinar um modelo de reconhecimento facial com imagens de rostos conhecidos, para que seja possível comparar o rosto capturado na imagem com os rostos conhecidos no modelo e identificar a pessoa.

## Resposta do servidor
Com base na identificação da pessoa, o servidor pode enviar uma resposta ao ESP-CAM, indicando se o rosto foi reconhecido ou não. Essa resposta pode ser enviada utilizando uma resposta HTTP ou uma mensagem MQTT para o ESP-CAM.

## Ações no ESP-CAM
Com base na resposta recebida do servidor, o ESP-CAM pode executar ações correspondentes. Por exemplo, se o rosto for reconhecido, o ESP-CAM pode abrir uma fechadura, acender uma luz ou realizar qualquer outra ação programada.

