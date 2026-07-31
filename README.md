# Concierge AR
Aplicação Web de Realidade Aumentada (WebXR) que permite explorar cardápios de restaurantes e visualizar seus modelos 3D diretamente no ambiente físico do usuário, usando a câmera do smartphone.

## Como funciona? 
1. Landing page (index.html) apresenta o projeto e leva o usuário ao cardápio.
2. Cardápio (cardapio.html) lista os restaurantes parceiros, com filtros por categoria e dois atalhos por card:
  - EXPERIÊNCIA AR → abre ar.html carregando o modelo .glb correspondente.
  - VER NO MAPS → abre a localização do restaurante no Google Maps.
3. Experiência AR (ar.html) usa a WebXR Device API + Three.js para:
  - Iniciar uma sessão immersive.ar.
  - Fazer hit-test no ambiente real, exibindo um retículo de referência.
  - Posicionar o modelo 3D do restaurante no ponto detectado.

## Tecnologias utilizadas:
- Three.js.
- WebXR Devide API.
- Node.js.
- HTML/CSS/JavaScript.

  ## Pré-requisitos:
  - Node.js instalado.
  - Um dispositivo compatível com ARCore.
  - Certificados key.pem e cert.pem na raiz do projeto.
 
  ### Gerando um certificado autoassinado:
  openssl req -nodes -new -x509 -keyout key.pem -out cert.pem -days 365

  ### Rodando o projeto:
  node server.js

  ## Créditos dos modelos:
  - "Japanese Restaurant "Inakaya"" (https://skfb.ly/6A6Yv) by Jellepostma is licensed under Creative Commons Attribution (http://creativecommons.org/licenses/by/4.0/).
  - "Restaurant" (https://skfb.ly/6RKF8) by Amy is licensed under Creative Commons Attribution (http://creativecommons.org/licenses/by/4.0/).
  - "Minecraft FNAF - Pizzeria" (https://skfb.ly/pzFOV) by Zero is licensed under Creative Commons Attribution (http://creativecommons.org/licenses/by/4.0/).
  - "Candy Shop Draft" (https://skfb.ly/6SrYC) by Rixael is licensed under Creative Commons Attribution (http://creativecommons.org/licenses/by/4.0/).
