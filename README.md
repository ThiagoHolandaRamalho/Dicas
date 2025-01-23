# Dicas

# Poetry 

1.autoriza o poetry gerenciar os ambientes virtuais: <pre><code>**poetry config virtualenvs.in-project true**</code></pre>

2.Cria novo projeto: <pre><code> **poetry new "nome do projeto"**</code></pre>

3.inicializa o poetry em um projeto existente: <pre><code> **poetry init**</code></pre>

4.Determnina a versão do pyhton que será utilizada no projeto: <pre><code> **pyenv local "3.*.*.*"**</code></pre>

5.Cria o ambiente virtual: <pre><code>**poetry env use "3.*.*.*"**</code></pre>

6.Instala as dependências do arquivo .toml: <pre><code>**poetry install --no-root**</code></pre>

# Formatadores de código
1. black
2. flake8
3. isort

criar o arquivo **.flake8** e adicionar as exceções 
  ![image](https://github.com/user-attachments/assets/bb2e8388-4f70-4445-905d-3352aca9665d)



# pre-commit

1.Instalar o pre-commit : **poetry add pre-commit**
2.Criar o arquivo: **.pre-commit-config.yaml**
3.Exemplo de hook utilizando as ferramentas de formatação:
<pre>
  <code>
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.5.0
    hooks:
      - id: trailing-whitespace
        args: [--markdown-linebreak-ext=md]
      - id: end-of-file-fixer
      - id: check-yaml
      - id: check-toml
      - id: detect-private-key
      - id: check-added-large-files
  - repo: https://github.com/psf/black-pre-commit-mirror
    rev: 24.1.1
    hooks:
      - id: black
        language_version: python3.11
  - repo: https://github.com/pycqa/isort
    rev: 5.13.2
    hooks:
      - id: isort
        name: isort (python)
  - repo: https://github.com/pycqa/flake8
    rev: 7.0.0
    hooks:
      - id: flake8
  </code>
</pre>

