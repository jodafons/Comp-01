
# 1) Criação da Virtual Environ:

Um Python Virtual Environment, também conhecido como `vitualenv`, é uma ferramenta essencial para desenvolvedores Python que desejam gerenciar dependências de projetos de forma eficiente e isolada. Com o `virtualenv`, você pode criar ambientes virtuais isolados para cada projeto, garantindo que as dependências específicas de cada projeto não interfiram umas nas outras.

Além disso, essa estratégia de desenvolvimento garante:
- *Isolamento de dependências*: Cada projeto pode ter suas próprias dependências, sem afetar outros projetos.
- *Gerenciamento de versões*: Você pode especificar a versão exata de cada dependência para cada projeto.
- *Reprodução de ambientes*: É fácil replicar o ambiente de desenvolvimento em diferentes máquinas ou ambientes.


## 1.1) Instalando o Virtualenv no Linux (Ubuntu/Debian)

1. *Atualize o índice de pacotes*: Execute o comando `sudo apt update`.
2. *Instale o Virtualenv*: Execute o comando `sudo apt install -y python3-virtualenv`.

Agora que você tem o Virtualenv instalado, pode criar ambientes virtuais para seus projetos Python e gerenciar dependências de forma eficiente.

> [!NOTE]
> *Verifique a versão*: Execute o comando `virtualenv --version` para verificar se a instalação foi bem-sucedida.


## 1.2) Como criar um Virtualenv?

1. *Abra o terminal*: Navegue até o diretório do seu projeto.
2. *Crie o vitualenv*: Execute o comando `virtualenv -p python nome_do_ambiente` (substitua "nome_do_ambiente" pelo nome desejado).
3. *Ative o venv*: Execute o comando `source nome_do_ambiente/bin/activate` (no Linux/Mac).
4. *Requerimentos de projeto*: Coloque todos os pacotes utilizados em seu projeto dentro do arquivo `requirements.txt`
5. *Instale dependências*: Use o comando `pip install -r requirements.txt` para instalar as dependências necessárias para o seu projeto.

> [!NOTE]
> Também é possível instalar os pacotes manualmente utilizando o comando `pip install nome_do_pacote_a nome_do_pacote b...`


## 1.3) Criando um Virtualenv com Jupyter Notebook Instalado

Aqui está um guia passo a passo para criar um virtualenv com Jupyter Notebook instalado:

Primeiro, abra o terminal e navegue até o diretório onde deseja criar o virtualenv.
Execute o comando 

```
virtualenv -p python jupyterlab
```

Observe que `jupyterlab` é o nome do ambiente que será utilizado nesse projeto. Por fim, ative o ambiente com o seguinte comando:

```
source jupyterlab/bin/activate
```

Após criar sua área de desenvolvimento com o `virtualenv`, crie um arquivo chamado `requirements.txt`. 
Dentro desse aquivo, insira as seguintes linhas:

```
pandas
numpy
juyterlab
```

Finalmente, instale os requerimentos dentro projeto.

```
pip install -r requirements.txt
```

Após instalar todos os pacotes desejados, verifique as versões dos pacotes com:

```
pip list
```



# 2) Utilização do Pip:

*O que é o pip?* O `pip` é o gerenciador de pacotes padrão para a linguagem de programação Python. Ele permite que você instale, atualize e remova pacotes Python de forma fácil e eficiente.

## 2.1) Principais recursos do pip
- *Instalação de pacotes*: O pip permite que você instale pacotes Python a partir do Python Package Index (PyPI) ou de outros repositórios.
- *Gerenciamento de dependências*: O pip gerencia as dependências dos pacotes, garantindo que todas as dependências necessárias sejam instaladas.
- *Atualização de pacotes*: O pip permite que você atualize pacotes para as versões mais recentes.
- *Remoção de pacotes*: O pip permite que você remova pacotes que não são mais necessários.

## 2.2) Comandos básicos do pip
- *Instalação*: `pip install nome_do_pacote`
- *Atualização*: `pip install --upgrade nome_do_pacote`
- *Remoção*: `pip uninstall nome_do_pacote`
- *Listagem de pacotes*: `pip list`

## 2.3) *O que é o pip freeze?*

 O `pip freeze` é um comando que lista todos os pacotes Python instalados no ambiente atual, junto com suas versões específicas. Ele é frequentemente usado para gerar um arquivo de requisitos (`requirements.txt`) que pode ser usado para replicar o ambiente em outra máquina ou projeto. Como usar o pip freeze?

- *Gerar arquivo de requisitos*: Execute o comando `pip freeze > requirements.txt` para gerar um arquivo `requirements.txt` com a lista de pacotes instalados.
- *Instalar pacotes*: Execute o comando `pip install -r requirements.txt` para instalar os pacotes listados no arquivo `requirements.txt`.

Com o `pip freeze`, você pode gerenciar dependências de projetos de forma eficiente e replicar ambientes com facilidade.


# 3) Notebooks

*O que é o Jupyter Notebook?*

O `Jupyter Notebook` é uma ferramenta de código aberto que permite criar e compartilhar documentos que contenham código, equações, visualizações e texto narrativo. É amplamente utilizado em ciência de dados, educação e pesquisa.

## 3.1) Principais recursos do Jupyter Notebook
- *Células de código*: Execute código em diferentes linguagens, incluindo Python, R e Julia.
- *Visualização de dados*: Inclua gráficos, imagens e outros elementos visuais para ilustrar seus dados.
- *Texto narrativo*: Adicione texto para explicar seu código e resultados. Em geral em linguagem do tipo `markdown`.
- *Compartilhamento*: Compartilhe seus notebooks com outros usuários.


## 3.2) Iniciando o Jupyter Notebook

1. *Inicie o Jupyter Notebook*: Execute o comando `jupyter-lab`.
2. *Acesse o Jupyter Notebook*: Abra um navegador e acesse a URL `http://localhost:8888`.

Agora você tem um virtualenv com Jupyter Notebook instalado e pronto para uso. Você pode criar notebooks e trabalhar em seus projetos Python de forma isolada e eficiente.

> [!WARNING]
> Para criar um servidor `jupyter` sem a necessidade de token, utilize a seguinte linha de comando 
>
> ```
> jupyter-lab --NotebookApp.token=''
> ```
>
