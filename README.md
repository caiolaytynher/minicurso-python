# Ambientes virtuais

## Criação

O último argumento é o nome do ambiente virtual. Em linhas gerais, o comando
está dizendo: Python, execute o módulo (por isso o `-m`) `venv` e dê o nome de
`.venv` para o ambiente virtual.

```shell
python -m venv .venv
```

## Ativação

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

```shell
pip install -r requirements.txt
```

Se você precisar atualizar as bibliotecas

```shell
pip install -r requirements.txt --upgrade
```
