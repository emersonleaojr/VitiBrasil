# API - Vitibrasil Embrapa 

Esse projeto foi desenvolvido para atender aos objetivos do Tech Challenge da Fase 1 da Pós Graduação em Machine Learning Engineering, turma 3MLET. 

### Objetivo

O trabalho envolve analisar os dados de vitivinicultura da Embrapa entre os anos de 1970 e 2023, os quais estão disponíveis na seguinte URL: [Vitibrasil Embrapa](http://vitibrasil.cnpuv.embrapa.br/index.php?).

A ideia do projeto é a criação de uma API pública de consulta nos dados do site nas respectivas abas:

-   /produção/{ano de interesse}
-   /processamento/{ano de interesse}
-   /comercialização/{ano de interesse}
-   /importação/{ano de interesse}
-   /exportação/{ano de interesse}

##  Configuração e Execução

1.  Clone o repositório:
```bash
https://github.com/emersonleaojr/VitiBrasil.git
```
2.  Crie e ative o ambiente virtual:
```bash
python3 -m venv venv
source venv/bin/activate
```

No Windows, utilize:
```bash
python -m venv venv
.venv\Scripts\activate
```
3.  Instale as dependências:
```bash
pip install -r requirements.txt
```

5.  Executando a Aplicação Localmente:
```bash
python3 main.py
```

Ou no Windows:
```bash
python main.py
```
Acesse a documentação da API no navegador: http://localhost:5000/apidocs ou http://127.0.0.1:5000/apidocs

### Pré-requisitos
-   Python 3.12 ou superior
-   Git
-   Ambiente virtual Python


## Dependências
- Flask
- Flasgger
- Requests
- BeautifulSoup4


## Estrutura atual do projeto

```bash
VitiBrasil/
├─ .vercel/
│  ├─ project.json
│  ├─ README.txt
├─ api/
│  ├─ routes/
│  │  ├─ routes.py
│  ├─ scraping/
│  │  ├─ comercializacao.py
│  │  ├─ exportacao.py
│  │  ├─ importacao.py
│  │  ├─ procesamento.py
│  │  ├─ producao.py
│  │  ├─ scraping.py
│  ├─ app.py
├─ .gitignore
├─ README.md
├─ requirements.txt
├─ vercel.json

```

### Deploy no Vercel

Para acessar o deploy no Vercel, clique [aqui](https://viti-brasil-api.vercel.app/).

## Contribuição

1.  Faça um fork do projeto.
2.  Crie uma branch para sua feature (`git checkout -b feature/SuaFeature`).
3.  Faça commit das suas alterações (`git commit -m 'Add Feature'`).
4.  Envie para a branch (`git push origin feature/SuaFeature`).
5.  Abra um Pull Request.
