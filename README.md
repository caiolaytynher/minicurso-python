# Ambientes virtuais

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
