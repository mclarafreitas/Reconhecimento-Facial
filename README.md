#Reconhecimento Facial

Projeto final da matéria Tópicos Avançados em Informática I do curso Bacharelado em Ciências e Tecnologia da Universidade Federal do Rio Grande do Norte (UFRN)

Professor:
  - Orivaldo

Alunos:
  - Maria Clara Moura de Freitas
  - Yuri
  
https://colab.research.google.com/drive/10GoMTYJk5gujUdmGI1nE0sJ558GaQtCW#scrollTo=I5b9emBxoPs4

Configuração do ESP-CAM
O objetivo deste projeto é realizar o reconhecimento facial utilizando um ESP-CAM, Python e um servidor. O ESP-CAM é conectado a um microcontrolador ESP8266 ou ESP32 e é necessário ter a biblioteca adequada para acessar a câmera. Além disso, a configuração da conexão Wi-Fi no ESP-CAM é fundamental para que ele possa se conectar ao servidor.

Captura da imagem
Para capturar a imagem, é necessário utilizar a biblioteca apropriada no microcontrolador que permita acessar a câmera do ESP-CAM. Com a biblioteca configurada, é possível capturar a imagem e salvá-la no microcontrolador para uso posterior.

Envio da imagem para o servidor
A imagem capturada precisa ser enviada para o servidor para processamento. Isso é feito estabelecendo uma conexão entre o ESP-CAM e o servidor, utilizando o protocolo HTTP ou MQTT. Através dessa conexão, a imagem capturada é enviada ao servidor para que possa ser processada.

Processamento da imagem no servidor
No servidor, é utilizado o Python para receber a imagem enviada pelo ESP-CAM. Para realizar o reconhecimento facial, bibliotecas como OpenCV, dlib ou TensorFlow são empregadas para processar a imagem. É necessário treinar um modelo de reconhecimento facial com imagens de rostos conhecidos, para que seja possível comparar o rosto capturado na imagem com os rostos conhecidos no modelo e identificar a pessoa.

Resposta do servidor
Com base na identificação da pessoa, o servidor pode enviar uma resposta ao ESP-CAM, indicando se o rosto foi reconhecido ou não. Essa resposta pode ser enviada utilizando uma resposta HTTP ou uma mensagem MQTT para o ESP-CAM.

Ações no ESP-CAM
Com base na resposta recebida do servidor, o ESP-CAM pode executar ações correspondentes. Por exemplo, se o rosto for reconhecido, o ESP-CAM pode abrir uma fechadura, acender uma luz ou realizar qualquer outra ação programada.

Este é um resumo básico do processo de reconhecimento facial utilizando o ESP-CAM, Python e um servidor. É importante ressaltar que a implementação real pode exigir ajustes e detalhes adicionais, como configuração da câmera, comunicação segura, gestão de erros, entre outros. Portanto, é necessário explorar e adaptar as bibliotecas específicas utilizadas para atender às necessidades do projeto.
