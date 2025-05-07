# Meu projeto

# Guia Básico de Git para o Projeto

Este documento explica os comandos Git utilizados no seu projeto, executados no terminal do macOS. Tambémm com o print de cada comando, e ao final a imagem do terminal

## Inicialização do Projeto

1. **Navegar até a pasta do projeto**:
   ```bash
   cd Documents/IF/semestre7/web
   ```

2. **Criar pasta do projeto**:
   ```bash
   mkdir meu-projeto
   cd meu-projeto
   ```

3. **Inicializar repositório Git**:
   ```bash
   git init
   ```
   - Cria um novo repositório Git na pasta
   - O Git sugere usar um nome diferente de 'master' para o branch principal

## Primeiro Commit

1. **Criar README.md**:
   ```bash
   echo "# Meu projeto" > README.md
   ```

2. **Verificar status**:
   ```bash
   git status
   ```

3. **Adicionar arquivo ao staging**:
   ```bash
   git add README.md
   ```

4. **Fazer primeiro commit - escrevi errado o first**:
   ```bash
   git commit -m "Fist commit: Adding readme.md"
   ```

## Configurar Repositório Remoto

1. **Adicionar origem remota**:
   ```bash
   git remote add origin https://github.com/Henrique-Jost/uni-intro-git.git
   ```

2. **Enviar para o repositório remoto**:
   ```bash
   git push -u origin master
   ```
   - Observe que inicialmente houve erro ao tentar usar 'main' (o branch local é 'master')

## Trabalhando com Branches

1. **Criar novo branch para feature**:
   ```bash
   git checkout -b feature/nova-funcionalidade
   ```

2. **Desenvolver a feature**:
   ```bash
   echo "Nova funcionalidade em desenvolvimento" > nova-funcionalidade.txt
   git add nova-funcionalidade.txt
   git commit -m "Adiciona nova funcionalidade"
   ```

3. **Enviar branch para o repositório remoto**:
   ```bash
   git push -u origin feature/nova-funcionalidade
   ```

## Integração de Mudanças

1. **Voltar para o branch master**:
   ```bash
   git checkout master
   ```

2. **Atualizar branch local**:
   ```bash
   git pull origin master
   ```

3. **Merge da feature**:
   ```bash
   git merge feature/nova-funcionalidade
   ```

4. **Enviar mudanças para o remoto**:
   ```bash
   git push origin master
   ```
# Imagens


