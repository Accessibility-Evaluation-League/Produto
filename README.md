# Acessibilidade Digital no Consumo de Medicamentos: Avaliação de Aplicativos de Farmácia (Estudo 4)

Este repositório contém os materiais e dados do Estudo 4 do artigo “Acessibilidade Digital no Ciclo de Consumo de Fármacos: Do Acesso à Informação ao Reconhecimento de Medicamentos por IAs Generativas” 


## Sobre o Estudo 4

O Estudo teve como objetivo analisar a acessibilidade dos três aplicativos de farmácia mais baixados no Brasil (identificados como P, D e DS) para dispositivos Android. 

A pesquisa focou em simular a jornada de compra de medicamentos por Pessoas com Deficiência Visual (PDVs), buscando identificar barreiras que impedem a autonomia desses usuários. O estudo utilizou uma abordagem qualiquantitativa, combinando ferramentas de inspeção automática com avaliações manuais realizadas por especialistas com e sem deficiência visual.

Os resultados revelaram um cenário crítico: foram identificadas mais de 5.000 violações de acessibilidade nos três aplicativos analisados. As falhas variaram desde a ausência de audiodescrição em imagens até problemas de semântica que impediam o uso de leitores de tela em funções básicas, como a barra de busca. Este repositório compartilha a metodologia e os dados gerados para que desenvolvedores e pesquisadores possam aprender com essas falhas e criar interfaces de saúde mais inclusivas.


## Conteúdo do Repositório

**Neste repositório, você encontrará:**

* Roteiro de Inspeção Manual: Uma planilha detalhada com 29 requisitos de acessibilidade (identificados de R02 a R47), baseados nas diretrizes da WCAG e adaptados para o contexto mobile.

* Guia da Jornada do Usuário: O detalhamento das 7 etapas de interação avaliadas:

- Navegação na Home;

- Fluxo de Login/Cadastro;

- Busca de Medicamentos;

- Análise da Lista de Resultados;

- Visualização de Detalhes do Produto;

- Gerenciamento do Carrinho;

- Endereço.


**Dados de Inspeção Automática**: Relatórios gerados pela ferramenta Accessibility Scanner, destacando erros de contraste, áreas de toque inadequadas e falta de rótulos.

**Relatos de Experiência (UX)**: Compilado de feedbacks qualitativos dos avaliadores PDVs, descrevendo a frustração e a perda de autonomia causadas por barreiras específicas, como botões com nomes técnicos ("BTN cesta home") ou feedbacks sonoros inexistentes.

### Ferramentas Utilizadas no Estudo

Para replicar ou expandir esta avaliação, foram utilizadas as seguintes tecnologias:

* **TalkBack:** Leitor de tela nativo do sistema Android para navegação descritiva.

* **Accessibility Scanner:** Ferramenta do Google para identificação automática de melhorias de acessibilidade em apps Android.

* **Planilha de Requisitos de Acessibilidade:** Instrumento metodológico para inspeção manual guiada.


## Objetivo

O propósito deste guia é fornecer recursos práticos para que a comunidade de desenvolvimento de software e Interação Humano-Computador (IHC) possa garantir que os serviços de saúde digitais sejam acompanhados de garantias efetivas de acessibilidade, promovendo autonomia e segurança para todos os usuários.
