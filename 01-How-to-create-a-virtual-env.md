# 01 Criação da Virtual Environ:

Um Python Virtual Environment, também conhecido como `vitualenv`, é uma ferramenta essencial para desenvolvedores Python que desejam gerenciar dependências de projetos de forma eficiente e isolada. Com o `virtualenv`, você pode criar ambientes virtuais isolados para cada projeto, garantindo que as dependências específicas de cada projeto não interfiram umas nas outras.

## Por que usar um vitualenv?

- *Isolamento de dependências*: Cada projeto pode ter suas próprias dependências, sem afetar outros projetos.
- *Gerenciamento de versões*: Você pode especificar a versão exata de cada dependência para cada projeto.
- *Reprodução de ambientes*: É fácil replicar o ambiente de desenvolvimento em diferentes máquinas ou ambientes.

## Instalando o Virtualenv no Linux (Ubuntu/Debian)

1. *Atualize o índice de pacotes*: Execute o comando `sudo apt update`.
2. *Instale o Virtualenv*: Execute o comando `sudo apt install -y python3-virtualenv`.

### Verificando a instalação
1. *Verifique a versão*: Execute o comando `virtualenv --version` para verificar se a instalação foi bem-sucedida.

Agora que você tem o Virtualenv instalado, pode criar ambientes virtuais para seus projetos Python e gerenciar dependências de forma eficiente.


## Como criar um virtualenv?

1. *Abra o terminal*: Navegue até o diretório do seu projeto.
2. *Crie o vitualenv*: Execute o comando `python -m venv nome_do_ambiente` (substitua "nome_do_ambiente" pelo nome desejado).
3. *Ative o venv*: Execute o comando `nome_do_ambiente\Scripts\activate` (no Windows) ou `source nome_do_ambiente/bin/activate` (no Linux/Mac).
4. *Instale dependências*: Use o comando `pip install` para instalar as dependências necessárias para o seu projeto.


## *Criando um Virtualenv com Jupyter Notebook Instalado*

Aqui está um guia passo a passo para criar um virtualenv com Jupyter Notebook instalado:

### Criando o Virtualenv
1. *Abra o terminal*: Navegue até o diretório onde deseja criar o virtualenv.
2. *Crie o virtualenv*: Execute o comando `virtualenv meu_ambiente` (substitua "meu_ambiente" pelo nome desejado).
3. *Ative o virtualenv*: Execute o comando `source meu_ambiente/bin/activate` (no Linux/Mac) ou `meu_ambiente\Scripts\activate` (no Windows).

# Instalando o Jupyter Notebook
1. *Instale o Jupyter Notebook*: Execute o comando `pip install jupyter-lab`.
2. *Verifique a instalação*: Execute o comando `jupyter-lab --version` para verificar se a instalação foi bem-sucedida.

# Iniciando o Jupyter Notebook
1. *Inicie o Jupyter Notebook*: Execute o comando `jupyter-lab`.
2. *Acesse o Jupyter Notebook*: Abra um navegador e acesse a URL `http://localhost:8888`.

Agora você tem um virtualenv com Jupyter Notebook instalado e pronto para uso. Você pode criar notebooks e trabalhar em seus projetos Python de forma isolada e eficiente.
