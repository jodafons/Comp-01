
# 01 Criação da Virtual Environ:

## Sumário

term
: Instalando o Virtualenv no Linux (Ubuntu/Debian) 


> [!WARNING]
> ssss


Um Python Virtual Environment, também conhecido como `vitualenv`, é uma ferramenta essencial para desenvolvedores Python que desejam gerenciar dependências de projetos de forma eficiente e isolada. Com o `virtualenv`, você pode criar ambientes virtuais isolados para cada projeto, garantindo que as dependências específicas de cada projeto não interfiram umas nas outras.

Além disso, essa estratégia de desenvolvimento garante:
- *Isolamento de dependências*: Cada projeto pode ter suas próprias dependências, sem afetar outros projetos.
- *Gerenciamento de versões*: Você pode especificar a versão exata de cada dependência para cada projeto.
- *Reprodução de ambientes*: É fácil replicar o ambiente de desenvolvimento em diferentes máquinas ou ambientes.

## Instalando o Virtualenv no Linux (Ubuntu/Debian)

1. *Atualize o índice de pacotes*: Execute o comando `sudo apt update`.
2. *Instale o Virtualenv*: Execute o comando `sudo apt install -y python3-virtualenv`.

> *Verifique a versão*: Execute o comando `virtualenv --version` para verificar se a instalação foi bem-sucedida.

Agora que você tem o Virtualenv instalado, pode criar ambientes virtuais para seus projetos Python e gerenciar dependências de forma eficiente.


## Como criar um Virtualenv?

1. *Abra o terminal*: Navegue até o diretório do seu projeto.
2. *Crie o vitualenv*: Execute o comando `virtualenv -p python nome_do_ambiente` (substitua "nome_do_ambiente" pelo nome desejado).
3. *Ative o venv*: Execute o comando `source nome_do_ambiente/bin/activate` (no Linux/Mac).
4. *Requerimentos de projeto*: Coloque todos os pacotes utilizados em seu projeto dentro do arquivo `requirements.txt`
5. *Instale dependências*: Use o comando `pip install -r requirements.txt` para instalar as dependências necessárias para o seu projeto.


## Criando um Virtualenv com Jupyter Notebook Instalado

Aqui está um guia passo a passo para criar um virtualenv com Jupyter Notebook instalado:

### Criando o Virtualenv
1. *Abra o terminal*: Navegue até o diretório onde deseja criar o virtualenv.
2. *Crie o virtualenv*: Execute o comando `virtualenv jupyter-env` (onde `jupyter-env` é o nome do ambiente escolhido).
3. *Ative o virtualenv*: Execute o comando `source jupyter-env/bin/activate` (no Linux/Mac).

### Criando um arquivo de *requirements*:

Primeiro, crie um arquivo chamado `requirements.txt`. Dentro desse aquivo, insira as seguintes linhas:

```
pandas
numpy
juyter-lab
```

Finalmente, instale os requerimentos dentro projeto.

```
pip install -r requirements.txt
```

Após instalar todos os pacotes desejados, verifique as versões dos pacotes com:

```
pip list
```

### Iniciando o Jupyter Notebook
1. *Inicie o Jupyter Notebook*: Execute o comando `jupyter-lab`.
2. *Acesse o Jupyter Notebook*: Abra um navegador e acesse a URL `http://localhost:8888`.

Agora você tem um virtualenv com Jupyter Notebook instalado e pronto para uso. Você pode criar notebooks e trabalhar em seus projetos Python de forma isolada e eficiente.
