**1 - Criar visitante**

Será usado a cada vez que um chat for aberto entre o cliente (médico generalista)  e a central. Informar o departamento que será chamado.

URL
/api/v1/livechat/visitor 
Método: POST

Passo a passo
https://blog.4linux.com.br/integrando-seu-chat-com-o-rocket-omnichannel/

Documentação da API
https://developer.rocket.chat/reference/api/rest-api/endpoints/omnichannel/livechat-endpoints/visitor/register-a-new-livechat-visitor


**2 - Criar sala**
Criar uma sala para o "visitante" (médico generalista) conversar com o atendente(médico especialista).
Configurar que a sala só pode ser criada se houver disponibilidde de um atendente (médico especialista) 

URL
/api/v1/livechat/room
Método: GET

Documentação da API
https://developer.rocket.chat/reference/api/rest-api/endpoints/omnichannel/livechat-endpoints/livechat-room/livechat-room-info


**3 - Enviar mensagens**
API para fazer o envio de mensagens do visitante para o atendente.

URL
/api/v1/livechat/message
Método: POST

Documentação da API
https://developer.rocket.chat/reference/api/rest-api/endpoints/omnichannel/livechat-endpoints/livechat-message/livechat-send-new-message


**4- Receber mensagem de volta do Rocket**
Receber as mensagens que o médico especialista enviar para o médico generalista.
Pode-se fazer por API ou por Webhook. Via API tem que efetuar constantes requisições para receber atualizações e tratar cada item da resposta individualmente. Não há possibilidade de filtros por apenas dados não vistos ou algo parecido, no máximo por eventos ocorridos após um timestamp informado. Resumindo, é mais complexo utilizar API e menos prático.

URL
/api/v1/livechat/messages.history/:rid
Método: POST

Dcumentação da API
https://developer.rocket.chat/reference/api/rest-api/endpoints/omnichannel/livechat-endpoints/livechat-message/load-livechat-messages-history

Por Webhook
No Rocket.chat ir em **Omnichannel** e clicar em **Webhooks**. Na tela aberta digitar o endereço para onde essas requisições serão disparadas e selecionar quais eventos deverão disparar essa ação.
Para cada evento, é realizada uma requisição **POST** para o endereço informado. O corpo da requisição varia em cada evento, mas é identificado o tipo do evento entre os campos.


**5 - Upload de arquivos**

Artigo:
https://docs.rocket.chat/guides/administration/settings/file-upload

Documentação da API
https://developer.rocket.chat/reference/api/rest-api/endpoints/team-collaboration-endpoints/rooms-endpoints/upload-file-to-a-room
Método: POST

Exemplos
com jscript
https://javascript.hotexamples.com/examples/meteor.rocketchat%3Afile-upload/FileUpload/-/javascript-fileupload-class-examples.html

com .net
https://stackoverflow.com/questions/57191015/how-to-upload-files-from-a-net-application-to-a-rocket-chat-channel
