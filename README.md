LenovoScraper

Automação para coleta e validação de especificações técnicas de notebooks Lenovo, com foco inicial nos modelos T14 G3, G4 e G5, e posteriormente expandido para outros modelos com variação no formato dos dados.

Funcionalidades

- Coleta automática de informações pelo número de série usando Selenium.
- Armazena os dados em arquivos `.txt` para posterior análise e exportação.
- Identifica campos com valores ausentes ("Não informado").
- Geração de logs para rastreabilidade.

Histórico do Projeto

O projeto começou com foco nos modelos T14 G3/G4/G5, que possuem estrutura padronizada. Com o tempo, notou-se que outros modelos exibiam informações de maneira distinta. Assim, foi criado um novo fluxo que salva os dados em `.txt` para posterior verificação dos padrões e exportação para Excel.

Tecnologias Utilizadas

Python 3
Selenium WebDriver
Jupyter Notebook
Pandas (para manipulação e exportação)
HTML/CSS (para exibição dos dados na intranet)



Como Executar

1. Instale os requisitos com:

```bash
pip install -r requirements.txt
```

2. Certifique-se de ter o ChromeDriver instalado e compatível com a versão do Google Chrome.

3. Execute a coleta:

Use os notebooks .ipynb para iniciar a extração com a lista de números de série.

A saída será salva em:

.txt (dados brutos),
.xlsx (planilha final),
.json (base para HTML dinâmico).


Público-Alvo
Equipe de Infraestrutura/Servidores: utiliza o Excel gerado.

Equipe de Front-End (TI): publica o HTML que lê os dados JSON.

Analistas Técnicos: podem revisar e adaptar o scraper para novos modelos.

Licença
Este projeto está licenciado sob os termos do arquivo LICENSE.