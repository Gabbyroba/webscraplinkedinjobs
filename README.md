# Automação de Coleta e Análise de Descrições de Vagas no LinkedIn

Este repositório contém um script Python que utiliza a biblioteca Selenium para automatizar a coleta de descrições de vagas de emprego no LinkedIn. As descrições são analisadas para criar uma nuvem de palavras que destaca os termos mais frequentes nas vagas.

## Pré-requisitos

Certifique-se de ter os seguintes componentes instalados:

- [Python](https://www.python.org/) (versão recomendada: 3.x)
- [Chromedriver](https://sites.google.com/chromium.org/driver/) - para controlar o navegador Chrome (verifique a versão compatível com o seu navegador)

## Instalação

1. Clone este repositório em seu ambiente local:

   ```bash
   git clone https://github.com/Gabbyroba/webscraplinkedinjobs.git
   ```

2. Navegue até o diretório clonado:

   ```bash
   cd webscraplinkedinjobs
   ```

3. Instale as bibliotecas Python necessárias usando o `pip`:

   ```bash
   pip install selenium beautifulsoup4 pandas wordcloud matplotlib
   ```

## Configuração

1. Substitua `email@mail,com` e `topsecret` pelo seu e-mail e senha do LinkedIn, respectivamente:

   ```python
   email = "seu-email@exemplo.com"
   password = "sua-senha"
   ```

2. Defina o cargo e a localização desejados para a pesquisa:

   ```python
   position = "analista de dados"
   local = "brazil"
   ```

3. Certifique-se de que o caminho para o arquivo `chromedriver.exe` está corretamente definido:

   ```python
   driver_path = "caminho/para/chromedriver.exe"
   ```

## Uso

1. Execute o script:

   ```bash
   python main.py
   ```

2. O script automatizará o processo de login no LinkedIn, pesquisa de vagas e coleta de descrições. Uma nuvem de palavras e um arquivo CSV contendo as descrições também serão gerados.

## Resultados

Após a execução do script, você encontrará os seguintes arquivos:

- `wordcloud-job.png`: Uma imagem da nuvem de palavras gerada a partir das descrições de vagas.
- `wordcloud-job.csv`: Um arquivo CSV contendo as descrições coletadas.

## Observações

- O uso de automação em sites pode violar os termos de uso. Use este script com responsabilidade e de acordo com as políticas do LinkedIn.
- Certifique-se de estar atualizado com as políticas de scraping e automação do LinkedIn.

## Contribuições

Contribuições são bem-vindas! Se você deseja melhorar ou estender este script, sinta-se à vontade para criar um "fork" deste repositório e enviar "pull requests".

