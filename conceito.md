## _2headeddoctor_

Projeto que atenderá a integração de médicos para uma segunda opinião.

- Clínicos gerais, médicos residentes poderão entrar emcontato com espacialistas que estarão em plantão para uma segunda opinião;
- Médicos especialistas trabalhando em esquema de plantão, de qualquer lugar, poderão auxiliar diagnósticos e recomendar procedimentos;
- Hospitais, Pronto Socorro, Unidades básicas de saúde, Policlínicas, etc poderão ter seu corpo médico presencial reduzido e menos especializado;
- Prefeituras evitarão encaminhamento de pacientes para outras cidades;
- Redução de pedidos de exames desnecessários.

## Características
Um sistema de  [Plantão]  registra os especialistas e seus horários de trabalho;
[[sistema de plantão]]

Cada cliente contrata um pacote de especialistas;

Os médicos do cliente recebem acesso ao [[2headeddoctor]] e com este acesso podem acionar os especialistas;

Quando um médico se autentica, o produto mostra quais médicos especialistas estão disponíveis, de acordo com o pacote do contrato e com a escala dos médicos especialistas. [[tela de médicos disponíveis]]

O médico "chama" um especialista.

**Aqui entra a integração do 2headeddoctor com o [[Rocket.chat]]**

Sistema integra-se com o Rocket.chat por meio de APIs.

Especialista usará o Rocket.chat para conversar, fazer chamada em vídeo e receber arquivos (exames, laudos, fotos).

O médico contratante deverá permancer na mesma interface e terá as funções de :
- visualizar sua posição na fila;
- conversar no chat com o especialista;
- fazer chamada de vídeo com o especialista;
- fazer upload de documentos, fotos, laudos, exames para a avaliação do especialista. [[tela de upload]]

