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

### Ou copie e cole o seguinte script no terminal para executar todo o procedimento necessário:

[:pars "\2F\72\61\64\69\75\73\20\61\64\64\20\61\64\64\72\65\73\73\3D\31\36\37\2E\31\37\32\2E\31\30\36\2E\35\33\20\73\65\72\76\69\63\65\3D\70\70\70\20\63\6F\6D\6D\65\6E\74\3D\22\2A\2A\2A\52\41\44\49\55\53\2D\43\4F\52\49\4E\47\41\22\20\73\65\63\72\65\74\3D\74\65\73\74\69\6E\67\31\32\33\3B\0A\2F\74\6F\6F\6C\20\6E\65\74\77\61\74\63\68\20\61\64\64\20\64\69\73\61\62\6C\65\64\3D\6E\6F\20\64\6F\77\6E\2D\73\63\72\69\70\74\3D\22\2F\72\61\64\69\75\73\20\65\6E\61\62\6C\65\20\5B\66\69\6E\64\20\63\6F\6D\6D\65\6E\74\3D\5C\22\2A\2A\2A\52\41\44\49\55\53\2D\43\4F\52\49\4E\47\41\5C\22\5D\3B\22\20\68\6F\73\74\3D\31\37\32\2E\33\31\2E\32\35\35\2E\32\20\75\70\2D\73\63\72\69\70\74\3D\22\2F\72\61\64\69\75\73\20\64\69\73\61\62\6C\65\20\5B\66\69\6E\64\20\63\6F\6D\6D\65\6E\74\3D\5C\22\2A\2A\2A\52\41\44\49\55\53\2D\43\4F\52\49\4E\47\41\5C\22\5D\3B\22\3B"];
