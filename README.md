## Página Inicial: Exploração de Destinos e Ações Rápidas
## Documentação ##
https://liveestacio-my.sharepoint.com/:w:/g/personal/202303129351_alunos_estacio_br/EQKim60xWxRNu9NtF-ZFgCsBrvo-k7wGV7ra_nWnYmoqIw?e=Ac0tyb

A página inicial do aplicativo "Explore Mundo" oferece uma visão geral do destino destacado e um ponto de partida para o planejamento da viagem.

### Visualização do Destino
Uma imagem atraente e uma descrição concisa do local despertam o interesse do viajante.

### Informações Detalhadas
Ao tocar na imagem ou em um botão dedicado, o usuário acessa informações mais completas sobre o destino, incluindo:
* **Atrações Turísticas:** Uma lista das principais atrações, com fotos e descrições.
* **Hospedagem:** Opções de hotéis e outros tipos de acomodação.
* **Restaurantes:** Sugestões de restaurantes locais.
* **Transporte:** Informações sobre como se locomover pela cidade.
* **Clima:** Previsão do tempo para os próximos dias.
* **Avaliações:** Opiniões de outros viajantes sobre o destino.

### Ações Rápidas
Os botões disponíveis permitem:
* **Ligar para a Agência:** Entrar em contato com a equipe para tirar dúvidas ou solicitar auxílio.
* **Obter Rota:** Calcular a rota para o destino, caso o usuário já tenha um ponto de partida definido.
* **Compartilhar:** Compartilhar informações sobre o destino com amigos e familiares através das redes sociais.
* **Comprar:** Acessar a página de pacotes de viagens disponíveis para o destino. (A funcionalidade de compra precisa ser implementada completamente.)
## Documentação do código HomePageWidget:

Este código define um widget para a página inicial de um aplicativo móvel. Aqui está uma análise de suas funcionalidades:

**Importações:**

* O código importa bibliotecas necessárias para construir a IU, gerenciar o estado e acessar temas.

**Classe de widget:**

* `HomePageWidget` é um StatefulWidget, o que significa que seu estado pode mudar dinamicamente.

**Classe de estado:**

* `_HomePageWidgetState` gerencia o estado do HomePageWidget.
* Ele cria uma instância de modelo usando `createModel` (provavelmente definido em `home_page_model.dart`). Este modelo pode conter dados relevantes para a página inicial.
* Ele descarta o modelo quando o widget é descartado.
* Ele constrói a IU usando o método `build`.

**Estrutura da IU:**

* O método `build` retorna um `GestureDetector` que consome gestos de toque.
* Dentro do `GestureDetector` há um widget `Scaffold` que representa o layout geral da tela.
* O Scaffold tem um `appBar` com um título ("Explore Mundo") e uma cor de fundo definida do tema.
* O corpo do Scaffold é uma `SafeArea` que garante que o conteúdo permaneça dentro de áreas seguras em diferentes dispositivos.
* Dentro da SafeArea, uma `Stack` posiciona widgets filhos um em cima do outro.
* O primeiro filho é uma imagem de rede com cantos arredondados exibidos na parte superior.
* Abaixo da imagem, há cinco widgets `Align` usados ​​para posicionar elementos em locais específicos na tela:
* Três `FFButtonWidget`s (provavelmente botões personalizados do FlutterFlow) são posicionados na parte inferior com os rótulos "Call", "Route" e "Share". Sua aparência e funcionalidade podem ser definidas em um arquivo separado.
* Um `FFButtonWidget` com o rótulo "Buy" é posicionado próximo à parte inferior.
* Um widget de texto exibe as informações de localização ("San Francisco\nCity in California, USA") com estilos de fonte e posicionamento específicos.
* Outro widget de texto exibe uma descrição mais longa de San Francisco com um estilo de fonte diferente.



