# Jovi Lens

Programa em Python que compara preços de produtos em lojas online. O usuário pode digitar o nome do produto ou escanear com a câmera, e o programa mostra as ofertas, indica a mais barata e permite salvar favoritos com alerta de queda de preço.

Projeto da Sprint 4 de Python.

## Funcionalidades

O programa abre um menu principal. Depois de cada opção, o usuário volta ao menu.

1. Escanear produto com a câmera
2. Buscar produto pelo nome
3. Meus favoritos
4. Verificar promoções
5. Histórico de alertas
6. Modo celular (usar a câmera do celular)
0. Sair

## Como executar

Requisitos: Python 3.9 ou superior e conexão com a internet. No Linux, instale também o Tkinter com `sudo apt install python3-tk`.

```bash
pip install -r requirements.txt
python main.py
```

## Configuração das chaves de API

Copie o arquivo `jovi_lens_config.example.json` para `jovi_lens_config.json` e preencha as chaves:

- `gemini_key`: identifica o produto pela foto (Google Gemini)
- `serper_key`: busca preços no Google Shopping (Serper)

As outras chaves são opcionais. Sem as chaves, a busca por nome usa a página pública do Mercado Livre, que pode bloquear o acesso.

O arquivo `jovi_lens_config.json` não é enviado ao Git.

## Persistência de dados

Os favoritos, o histórico de preços e os alertas são salvos em `jovi_lens_dados.json`, que é criado automaticamente.

## APIs utilizadas

- Mercado Livre
- Serper (Google Shopping)
- SerpAPI
- Google Gemini

## Estrutura

```
main.py                          programa principal
recursos/pagina_celular.html     página do modo celular
jovi_lens_config.example.json    modelo de configuração
requirements.txt                 dependências
```

## Integrantes

570881 - GABRIEL FREITAS DA SILVA CARVALHO
572892 - ERICK MARTINS PICOLO
572171 - GUILHERME MARCON DANTAS
569782 - LUIZ FELIPE CARDOSO DE OLIVEIRA
