# Microvolts Item Finder

Aplicação web estática para pesquisar itens do MicroVolts por tipo e consultar seus IDs.

## Requisitos

- [Git](https://git-scm.com/)
- [Python 3](https://www.python.org/downloads/) para iniciar um servidor HTTP local

Não é necessário instalar pacotes nem configurar variáveis de ambiente.

## Setup

Clone o repositório e acesse a pasta do projeto:

```bash
git clone https://github.com/ropehapi/microvolts-item-finder.git
cd microvolts-item-finder
```

Se o projeto já estiver no seu computador, basta abrir um terminal na pasta dele.

## Como rodar

Na raiz do projeto, inicie o servidor:

```bash
python3 -m http.server 8000
```

No Windows, caso `python3` não esteja disponível, use:

```powershell
py -m http.server 8000
```

Depois, acesse no navegador:

<http://localhost:8000>

Para encerrar o servidor, pressione `Ctrl+C` no terminal.

> Não abra o `index.html` diretamente. A aplicação carrega `items.json` e `icons.json` com `fetch`, que pode ser bloqueado pelo navegador quando não há um servidor HTTP.

## Uso

1. Abra a aplicação no navegador.
2. Escolha uma categoria em **Inventory Type**.
3. Consulte o nome, a descrição e os IDs dos itens exibidos.

## Estrutura principal

```text
index.html   # Estrutura da página
style.css    # Estilos da interface
script.js    # Carregamento, exibição e filtro dos itens
items.json   # Dados dos itens
icons.json   # Metadados dos ícones
icons/       # Imagens dos itens
```
