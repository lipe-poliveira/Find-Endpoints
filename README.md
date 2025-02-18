# Find-Endpoints - Escaneador de Recursos Web

## Descrição
Este script JavaScript tem como objetivo escanear recursos carregados em uma página web e extrair caminhos relativos encontrados dentro deles. Ele busca identificar links internos definidos no código fonte das respostas HTTP, como arquivos JavaScript, CSS e HTML. Os resultados são exibidos diretamente na página em um painel fixo na parte inferior.

## Funcionalidades
- **Coleta de Recursos**: Identifica e processa os recursos carregados na página.
- **Extração de Caminhos Relativos**: Filtra caminhos válidos que podem ser usados para navegação interna.
- **Interface Visual**: Exibe os resultados em um painel dinâmico na própria página.
- **Botão de Cópia**: Permite copiar os caminhos extraídos para a área de transferência.
- **Tratamento de Erros**: Captura falhas de carregamento e erros de requisição.

## Como Funciona
1. O script é executado automaticamente ao ser inserido em uma página.
2. Cria uma interface fixa no rodapé da tela.
3. Coleta todos os recursos carregados na página.
4. Faz requisições HTTP para obter o conteúdo dos recursos.
5. Analisa e extrai caminhos relativos de cada recurso processado.
6. Exibe os caminhos extraídos no painel.
7. Permite copiar os caminhos para a área de transferência com um botão.

## Tecnologias Utilizadas
- **JavaScript**: Manipulação da DOM, requisição de recursos e extração de dados.
- **CSS (Inline)**: Estilização do painel para exibição dos resultados.
- **Fetch API**: Para buscar e processar recursos carregados na página.

## Melhorias Implementadas
- Uso de **Set** para evitar repetição de URLs e caminhos.
- Melhor extração de caminhos, incluindo suporte a crases e remoção de query strings.
- Interface visual aprimorada com um painel responsivo.
- Feedback aprimorado na cópia dos resultados, com confirmação temporária no botão.
- Otimização da busca de recursos usando **Promise.all**.

## Como Usar
1. Insira o script em um console de desenvolvedor ou como um bookmarklet.
2. Aguarde a análise e extração dos caminhos.
3. Copie os resultados usando o botão exibido no painel.

## Exemplo de Uso
Caso esteja navegando em um site e queira encontrar todos os caminhos internos referenciados no código fonte, basta executar este script para obter a lista de caminhos de forma rápida e organizada.
