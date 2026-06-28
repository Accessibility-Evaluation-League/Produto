# Acessibilidade Digital no Consumo de Medicamentos: Avaliação de Aplicativos de Farmácia (Estudo 4)

Este repositório contém os materiais e dados do Estudo 4 do artigo “Avaliação de Acessibilidade Digital no Ciclo do Consumo de Fármacos” 


## Objetivo

O propósito deste repositório é fornecer recursos para auxiliar em pesquisas para que a comunidade de desenvolvimento de software e Interação Humano-Computador (IHC) possa garantir que os serviços de saúde digitais sejam acompanhados de garantias efetivas de acessibilidade, promovendo autonomia e segurança para todos os usuários.


## Sobre o Estudo 4

O Estudo teve como objetivo analisar a acessibilidade dos três aplicativos de farmácia mais baixados no Brasil (identificados como P, D e DS) para dispositivos Android. 

A pesquisa focou em simular a jornada de compra de medicamentos por Pessoas com Deficiência Visual (PDVs), buscando identificar barreiras que impedem a autonomia desses usuários. O estudo utilizou uma abordagem qualiquantitativa, combinando ferramentas de inspeção automática com avaliações manuais realizadas por especialistas com e sem deficiência visual.

Os resultados revelaram um cenário crítico: foram identificadas mais de 5.000 violações de acessibilidade nos três aplicativos analisados. As falhas variaram desde a ausência de audiodescrição em imagens até problemas de semântica que impediam o uso de leitores de tela em funções básicas, como a barra de busca. Este repositório compartilha a metodologia e os dados gerados para que desenvolvedores e pesquisadores possam aprender com essas falhas e criar interfaces de saúde mais inclusivas.


## Conteúdo do Repositório

**Neste repositório, você encontrará:**

* Roteiro de Inspeção Manual: Uma planilha detalhada com 29 requisitos de acessibilidade (identificados de R02 a R47), baseados nas diretrizes da WCAG e adaptados para o contexto mobile.

* Guia da Jornada do Usuário: O detalhamento das 7 etapas de interação avaliadas:
  
 1. Navegação na Home;
 2. Fluxo de Login/Cadastro;
 3. Busca de Medicamentos;
 4. Análise da Lista de Resultados;
 5. Visualização de Detalhes do Produto;
 6. Gerenciamento do Carrinho;
 7. Endereço.


**Dados de Inspeção Automática**: Relatórios gerados pela ferramenta Accessibility Scanner, destacando erros de contraste, áreas de toque inadequadas e falta de rótulos.

**Relatos de Experiência (UX)**: Compilado de feedbacks qualitativos dos avaliadores PDVs, descrevendo a frustração e a perda de autonomia causadas por barreiras específicas, como botões com nomes técnicos ("BTN cesta home") ou feedbacks sonoros inexistentes.

### Ferramentas Utilizadas no Estudo

Para replicar ou expandir esta avaliação, foram utilizadas as seguintes tecnologias:

* **TalkBack:** Leitor de tela nativo do sistema Android para navegação descritiva.

* **Accessibility Scanner:** Ferramenta do Google para identificação automática de melhorias de acessibilidade em apps Android.

* **Planilha de Requisitos de Acessibilidade:** Instrumento metodológico para inspeção manual guiada.



### Exemplos de erros nos aplicativos
Embora todos os aplicativos examinados apresentem falhas que podem interromper a jornada de compra de PDVs, o aplicativo P chama a atenção negativamente. Com um total de 2.909 erros detectados, destaca-se um problema extremamente crítico: a ausência de suporte para o TalkBack especificamente na barra de pesquisa, o que impede que o usuário consiga localizar ou buscar medicamentos, inviabilizando uma funcionalidade fundamental durante a navegação. 

**Barra de pesquisa do aplicativo P inacessível:**
Vídeo
https://github.com/user-attachments/assets/4d341571-96d2-482c-8fb4-ebf25b2b3e93

**Total de erros: **

<img width="784" height="206" alt="Total de erros" src="https://github.com/user-attachments/assets/f11a6ae6-0fad-4275-8c90-36e5cf686dd7" />



### Sugestões de melhoria pelos usuários

#### Avaliador 2

*   **Aplicativo DS:**
    *   **Melhoria na semântica:** Aprimorar a semântica geral do aplicativo para facilitar a compreensão por tecnologias assistivas.
    *   **Campos de cadastro:** Permitir a inserção de caracteres nos campos de cadastro e corrigir o redirecionamento automático indevido entre campos durante a digitação.
    *   **Resultados de busca:** Melhorar a descrição dos componentes de interface dos remédios, que estavam incompreensíveis.

*   **Aplicativo D:**
    *   **Nomenclatura de botões:** Incluir ou corrigir nomes em botões essenciais para a navegação (como o botão de "voltar"), que estavam ausentes ou incompreensíveis.
    *   **Pop-ups:** Gerenciar pop-ups de forma mais acessível, pois atrapalham a navegação.
    *   **Processo de cadastro:** Corrigir falhas no envio de códigos para login/cadastro via serviços externos (como Google).

*   **Aplicativo P:**
    *   **Campo de pesquisa:** Tornar o campo de busca clicável e acessível, pois não foi possível utilizá-lo.
    *   **Rótulos de botões:** Substituir nomenclaturas técnicas e incompreensíveis, como "BTN cesta home" e "BTN numerocomletras", por descrições claras da função do botão.

---

#### Avaliador 3

*   **Aplicativo D:**
    *   **Interface e Performance:** Otimizar o aplicativo para ser mais leve e garantir que as descrições de botões e componentes sejam precisas.
    *   **Fluxo de navegação:** Tornar a ordem das ações principais (do login ao carrinho) mais lógica, evitando a sensação de que são apenas ofertas publicitárias durante o percurso.
    *   **Carrinho e Checkout:** Corrigir a leitura de elementos identificados apenas como "Object" pelo TalkBack. Além disso, remover propagandas do carrinho e facilitar a ativação do botão de adicionar (atualmente dependente da seleção prévia de quantidade).

*   **Aplicativo DS:**
    *   **Remoção de barreiras:** Remover pop-ups que não possuem acessibilidade.
    *   **Nomenclaturas:** Corrigir nomenclaturas invertidas ou erradas, especialmente nos botões de "Favoritar/Desfavoritar" e "Compartilhar".
    *   **Feedback e Detalhes:** Ativar feedback sonoro para as ações do usuário e adicionar informações detalhadas do produto no carrinho para leitura pelo TalkBack.
    *   **Busca e Login:** Melhorar a compatibilidade da barra de busca e oferecer mais opções de login.

*   **Aplicativo P:**
    *   **Compatibilidade total:** Garantir a compatibilidade do leitor de tela com todos os elementos, especialmente a barra de pesquisa, que não era lida pelo TalkBack.
    *   **Rótulos de produtos:** Garantir que o nome dos produtos seja lido nos resultados de busca, eliminando rótulos genéricos como "BTN - número".
    *   **Feedback de ação:** Adicionar aviso sonoro ou feedback claro ao adicionar itens ao carrinho, para confirmar que a ação foi bem-sucedida.


