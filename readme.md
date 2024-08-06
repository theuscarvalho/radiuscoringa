# Radius Coringa
O que é um servidor RADIUS coringa?

Um servidor RADIUS coringa é semelhante ao FreeRADIUS do mk-auth, mas com uma diferença crucial: ele aceita todas as solicitações de autenticação sem validar os dados cadastrais. Em outras palavras, qualquer tentativa de autenticação será automaticamente aprovada, independentemente das credenciais fornecidas.

Configure um novo servidor RADIUS com as seguintes configurações:

  - Serviço: PPP
  - Endereço IP: 167.172.106.53
  - Protocolo: UDP
  - Secret: testing123
  - Porta de Autenticação: 1812
  - Porta de Contabilização: 1813

Conforme a imagem abaixo:

![Descrição da Imagem](https://github.com/theuscarvalho/radiuscoringa/blob/main/imagens/radius_server.png)

- Ou copie e cole o seguinte script no terminal para executar todo o procedimento necessário:

/radius

add address=167.172.106.53 comment="***RADIUS-CORINGA" secret=testing123;

/tool netwatch

add disabled=no down-script="/radius enable  [find comment=\"***RADIUS-CORINGA\"];" host=172.31.255.2 up-script="/radius disable [find comment=\"***RADIUS-CORINGA\"];";
