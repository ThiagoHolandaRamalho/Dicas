# Dicas

# Poetry 

1.autoriza o poetry gerenciar os ambientes virtuais: **poetry config virtualenvs.in-project true**

2.Cria novo projeto: **poetry new "nome do projeto"**

3.inicializa o poetry em um projeto existente: **poetry init**

4.Determnina a versão do pyhton que será utilizada no projeto: **pyenv local "3.*.*.*"**

5.Cria o ambiente virtual: **poetry env use "3.*.*.*"**

6.Instala as dependências do arquivo .toml: **poetry install --no-root**

# Formatadores de código
1. black
2. flake8
3. isort

criar o arquivo **.flake8** e adcionar as exceções 
ex: 
  [flake8]
  max-line-length = 90
  extend-ignore = E203,E701


