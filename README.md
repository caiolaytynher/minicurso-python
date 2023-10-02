# Ambientes virtuais

Para garantir que as bibliotecas utilizadas sejam instaladas de maneira isolada,
permitindo a fácil remoção de qualquer uma delas e permitindo a garantia de
funcionamento do gerenciador de pacotes, o Pip, os códigos serão executados
através de um executável local que faz parte de um **ambiente virtual**. O
próprio Python possui uma solução para criar estes ambientes, e à seguir veremos
como é feita a sua criação, ativação e utilização.

## Criação

O último argumento é o nome do ambiente virtual. Em linhas gerais, o comando
está dizendo: Python, execute o módulo (por isso o `-m`) `venv` e dê o nome de
`.venv` para o ambiente virtual.

```shell
python -m venv .venv
```

## Ativação

Antes de executar os programas, para que as bibliotecas instaladas no ambiente
virtual funcionem, é necessário ativa-lo dentro da sessão de terminal.

### Windows

Pode não funcionar no Powershell. Utilizar o Prompt de comando ou
permitir a execução de scripts nas configurações.

```shell
.\.venv\Scripts\activate
```

### Linux/MacOS

```shell
source .venv/bin/activate
```

## Atualizando pip

O gerenciador de pacotes do Python se chama Pip. Ele é o responsável por
instalar as bibliotecas. Quando se utiliza o Pip dentro de um ambiente virtual,
ele instala as bibliotecas dentro do ambiente de forma isolada.

```shell
pip install --upgrade pip
```

## Instalação de bibliotecas

Dentro dos arquivos de ajuda, existe um que se chama `requirements.txt`, que é
um arquivo de texto comum que contém o nome de todas as bibliotecas que serão
instaladas. Nada impede que a instalação seja feita manualmente, é apenas boa
prática manter um arquivo dizendo exatamente o que você instalou. Isso também
facilita o processo de atualização.

```shell
pip install -r requirements.txt
```

Se você precisar atualizar as bibliotecas

```shell
pip install -r requirements.txt --upgrade
```
