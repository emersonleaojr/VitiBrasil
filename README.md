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

## Estrutura atual do projeto

```
VitiBrasil/
├─ .vercel/
│  ├─ README.txt
│  ├─ vercel.json
├─ api/
│  ├─ routes/
│  │  ├─ routes.py
│  ├─ scraping/
│  │  ├─ comercializacao.py
│  │  ├─ exportacao.py
│  │  ├─ importacao.py
│  │  ├─ processamento.py
│  │  ├─ producao.py
│  │  ├─ scraping.py
│  ├─ app.py
├─ .gitignore
├─ README.md
├─ requirements.txt
├─ vercel.json
```

##  Configuração e Execução

1.  Clone o repositório:
```
https://github.com/emersonleaojr/VitiBrasil.git
```
2.  Crie e ative o ambiente virtual:
```
python3 -m venv venv
source venv/bin/activate
```

No Windows, utilize:
```
python -m venv venv
venv\Scripts\activate
```
3.  Instale as dependências:
```
pip install -r requirements.txt
```

5.  Executando a Aplicação Localmente (necessário instalar node.js):
```
npm i -g vercel
vercel dev
```

Acesse a documentação da API no navegador: http://localhost:3000/apidocs.

### Pré-requisitos
-   Python 3.12 ou superior
-   Git
-   Ambiente virtual Python
-   Node.js

### Dependências
- Flask
- Flasgger
- Requests
- BeautifulSoup4

## Deploy no Vercel

Para acessar o deploy no Vercel, clique [aqui](https://viti-brasil.vercel.app/).

## Possível aplicação para modelagem
![Fase_1_3MLET](https://github.com/user-attachments/assets/682cb513-1b90-45ed-a867-adaebcf5a925)

## Contribuição

1.  Faça um fork do projeto.
2.  Crie uma branch para sua feature (`git checkout -b feature/SuaFeature`).
3.  Faça commit das suas alterações (`git commit -m 'Add Feature'`).
4.  Envie para a branch (`git push origin feature/SuaFeature`).
5.  Abra um Pull Request.


