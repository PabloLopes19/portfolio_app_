# Hygge App

**Projeto:** Hygge: Poste e compartilhe suas viagens e experiências mundo a fora.
**Aluno:** Pablo Lopes
**Curso:** Engenharia de Software.
**Data:** 29 de março de 2025

---

# Resumo

O projeto é um aplicativo mobile voltado para entusiastas de viagens que desejam compartilhar suas experiências com o mundo. No app, os usuários podem criar postagens detalhadas sobre suas viagens, incluindo fotos, vídeos, itinerários e dicas sobre os lugares visitados. Além disso, eles podem seguir amigos, influenciadores e viajantes para acompanhar suas aventuras e descobrir novos destinos.

---

## 1. Introdução

A fim de construir uma aplicação mobile, que traga uma maneira nova das pessoas interagirem e compartilharem momentos e experiências, é proposto um aplicativo onde seja possível um usuário criar uma conta, fazer postagens, curtir e compartilhar viagens de outros usuários.

Então, com isso é criado o Hygge, nele é possível compartilhar e interagir com pessoas e suas experiências ao redor do globo. Para isso, foi optado por um aplicativo para dispositivos móveis, pois isso possibilita o acesso de um número maior de usuários, e facilita a criação e visualização dos posts uma vez que os usuários podem usar a aplicação de qualquer lugar.

---

## 2. Descrição do Projeto

Nas décadas recentes, redes sociais se tornaram o tipo de sistema mais popular entre a grande massa de usuários. Cada plataforma se propôs a criar um diferente experimento social humano. O tema escolido então, para este projeto é o de viagens. Considerando que a grande maioria das pessoas opta por fazer viagens em férias e no tempo livre. E a grande maioria das pessoas compartilha esses momentos com seus amigos e familiares através de redes sociais comuns, através de fotos com Instagram ou vídeos curtos com TikTok e YouTube Shorts ou até vídeos mais bem produzidos no YouTube.

---

## 3. Especificação Técnica

Com isso, nossa proposta é criar uma maneira das pessoas criarem um registro diferenciado de lugares e experiências que conheceram. Talvez uma pessoa queira conhecer um país específico, ele pode criar uma viagem, colocar os lugares onde quer conhecer e montar todo o plano de uma viagem e depois realizar esse sonho e compartilhar com seus seguidores.

Visando facilitar também a criação desses posts, sabendo que a digitação de longos textos e seleção de fotos é um trabalho desgastante para o usuário, tivemos a ideia de possibilitar o usuário a apenas fornecer as informações necessárias para montar todo o post utilizando Inteligência Artifical (IA). Podemos utilizar a IA em outras partes do aplicativo, visando em um primeiro momento, apenas a facilitação de criação dos usuários dentro do app.

### 3.1. Requisitos de Software

Pensando e oferecer ao usuário a possibilidade de criar suas viagens e compartilhar elas com as pessoas. Resumidamente então, podemos assumir que o sistema precisa de um sistema de autenticação para criar a sua conta, criar seus posts de maneira simples e intuitiva e ter uma aplicação segura e agradável de se usar.

#### Requisitos funcionais

**🧑‍🤝‍🧑 Perfil e Autenticação**

- RF001 - O usuário deve poder criar uma conta com e-mail/senha ou login social (Google, Facebook, Apple).
- RF002 - O usuário deve poder criar e editar seu perfil (nome, foto, bio, redes sociais, localização).
- RF003 - O usuário deve poder seguir e ser seguido por outros usuários.

**📸 Criação e Gerenciamento de Posts**

- RF004 - O usuário pode criar um post manualmente informando:
  - Nome do destino
  - Tipo de viagem (turismo, negócios, mochilão etc.)
  - Data da viagem (ou previsão de ida)
  - Roteiro (dia a dia, locais visitados)
  - Texto descritivo
  - Fotos e vídeos
  - Tags ou categorias
- RF005 - O usuário pode criar um post com ajuda da IA informando:
  - Destino
  - Duração da viagem
  - Objetivo ou estilo da viagem
  - Locais visitados
  - Impressões gerais
- RF006 - O sistema deve gerar automaticamente um texto base (com IA) com base nas informações fornecidas, para que o usuário edite antes de publicar.
- RF007 - O usuário pode visualizar, editar e excluir seus próprios posts.

**🔎 Exploração e Interações**

- RF008 - O usuário pode visualizar uma timeline com posts de outras pessoas.
- RF009 - O usuário pode curtir, comentar e compartilhar posts.
- RF010 - O usuário pode salvar posts em coleções personalizadas (ex: “Futuros destinos”).
- RF011 - O usuário pode pesquisar por destino, tag, nome de usuário ou tipo de viagem.

**📍 Funcionalidades de Localização**

- RF012 - O usuário pode marcar lugares no mapa (Google Maps/OpenStreetMap) em seus posts.
- RF013 - O app pode sugerir atrações baseadas no destino do post.
- RF014 - O app pode exibir um mapa interativo com todos os lugares visitados pelos usuários.

**✈️ Roteiros e Planejamento**

- RF015 - O usuário pode criar roteiros personalizados com base em dias, locais e atividades.
- RF016 - O usuário pode compartilhar roteiros com outros usuários ou torná-los públicos.

**🧠 Funcionalidades com IA**

- RF017 - A IA pode sugerir:
  - Texto automático para post
  - Títulos atrativos
  - Sugestões de tags e categorias
  - Melhoria de fotos (filtro, correção de cor etc., opcional)
  - RF018 - A IA pode gerar um roteiro base com base no destino informado.

#### 🚧 Requisitos Não-Funcionais

**🔐 Segurança e Privacidade**

- RNF001 - Os dados do usuário devem ser armazenados de forma segura (criptografia, JWT etc.).
- RNF002 - O sistema deve seguir boas práticas de proteção de dados (LGPD/GDPR).

**⚙️ Desempenho e Escalabilidade**

- RNF003 - O app deve carregar a timeline em até 2 segundos com boa conexão.
- RNF004 - A geração de texto com IA não deve ultrapassar 10 segundos de espera.
- RNF005 - O sistema deve ser escalável para suportar milhares de usuários simultaneamente.

**🧩 Manutenibilidade e Modularidade**

- RNF006 - O sistema deve ser modular para permitir a adição de novas funcionalidades, como pacotes turísticos ou integração com agências.
- RNF007 - A arquitetura deve permitir o desacoplamento entre frontend, backend e serviços de IA.

**📱 Compatibilidade**

- RNF008 - O app deve ser compatível com Android 8+ e iOS 13+.
- RNF009 - O design deve ser responsivo para diferentes tamanhos de tela.

**☁️ Armazenamento e Mídia**

- RNF010 - O upload de imagens e vídeos deve utilizar serviços como Firebase, S3 ou similares.
- RNF011 - As mídias devem ser otimizadas para consumo de dados reduzido sem comprometer a qualidade.

---

### 3.2. Considerações de Design

Discussão sobre as escolhas de design, incluindo alternativas consideradas e justificativas para as decisões tomadas. Visão Inicial da Arquitetura: Descrição dos componentes principais e suas interconexões. Padrões de Arquitetura: Indicação de padrões específicos utilizados (ex.: MVC, Microserviços). Modelos C4: Detalhamento da arquitetura em níveis: Contexto, Contêineres, Componentes, Código.

- Pq nativo?
- Comparação nativo com React Native e Flutter
- Comparação com KMP
- MVVM para Android e iOS

### 3.3. Stack Tecnológica

- Kotlin | Android
- Swift | iOS

### 3.4. Considerações de Segurança

Análise de possíveis questões de segurança e como mitigá-las.

---

## 4. Próximos Passos

Descrição dos passos seguintes após a conclusão do documento, com uma visão geral do cronograma para Portfólio I e II.

---

## 5. Referências

Listagem de todas as fontes de pesquisa, frameworks, bibliotecas e ferramentas que serão utilizadas.

---

## 6. Apêndices (Opcionais)

Informações complementares, dados de suporte ou discussões detalhadas fora do corpo principal.

---

## 7. Avaliações de Professores

Adicionar três páginas no final do RFC para que os Professores escolhidos possam fazer suas considerações e assinatura:

    Considerações Professor/a:
    Considerações Professor/a:
    Considerações Professor/a:
