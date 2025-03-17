# Guia Completo de Comandos Git 🚀

## 🔧 Configuração Inicial do Git

- 📝 `git config --global user.name "Seu Nome"` →                   #Define o nome do usuário.
- 📧 `git config --global user.email "seuemail@example.com"` →      #Define o e-mail do usuário.
- ❌ `git config --global --unset user.name` →                      #Remove a configuração global do nome do usuário.
- ❌ `git config --global --unset user.email` →                     #Remove a configuração global do e-mail do usuário.
- ⚙️ `git config --list` →                                          #Exibe as configurações do Git.
- 🌿 `git config --global init.defaultBranch <name>` →              #Define o nome padrão da branch inicial ao criar um novo repositório.
- ✏️ `git config --global core.editor "editor"` →                 #Define o editor de texto padrão para o Git.
- 📜 `git config --global core.pager cat` →                        #Define o pager padrão do Git para exibir saída diretamente no terminal.
- 🔑 `git config --global credential.helper store` →               #Armazena as credenciais do Git permanentemente.
- 📝 `git config --local user.name "Seu Nome"` →                  #Define o nome do usuário apenas para o repositório atual.
- 📧 `git config --local user.email "seuemail@example.com"` →     #Define o e-mail do usuário apenas para o repositório atual.
- 🔍 `git config --local user.name` →                              #Exibe o nome do usuário configurado localmente.
- 🔍 `git config --local user.email` →                             #Exibe o e-mail do usuário configurado localmente.

## 📂 Inicialização e Clonagem

- 🆕 `git init` →                                                  #Inicializa um repositório Git na pasta atual.
- 🔄 `git clone URL_DO_REPO` →                                     #Clona um repositório remoto para o computador.

## 🔑 Autenticação com GitHub CLI

- 🔐 `gh auth login` →                                            #Faz login no GitHub via linha de comando.
- 🚪 `gh auth logout` →                                           #Faz logout da conta do GitHub na linha de comando.

## 📜 Status e Histórico

- 🔍 `git status` →                                               #Mostra o status dos arquivos (modificados, adicionados, etc.).
- 📜 `git log` →                                                  #Exibe o histórico de commits.
- 📊 `git log --oneline --graph` →                               #Exibe um histórico resumido e visual.
- 📌 `git log --oneline` →                                       #Mostra o histórico de commits em uma única linha por commit.
- 🧐 `git log -p` →                                             #Exibe o histórico de commits com as diferenças de cada mudança.
- 📊 `git log --stat` →                                         #Mostra estatísticas das alterações em cada commit.
- 🔍 `git diff` →                                                #Exibe as diferenças entre os arquivos modificados e o último commit.
- 🔄 `git diff --cached` →                                       #Exibe as diferenças dos arquivos adicionados ao staging em relação ao último commit.

## 🛠️ Trabalhando com Arquivos

- ➕ `git add arquivo.txt` →                                     #Adiciona um arquivo específico ao staging.
- 📂 `git add .` →                                              #Adiciona **todos os arquivos** modificados ao staging.
- ✅ `git commit -m "Mensagem do commit"` →                     #Confirma as mudanças adicionadas.
- ✏️ `git commit --amend` →                                     #Modifica o último commit.
- 🔄 `git commit --amend --no-edit` →                          #Modifica o último commit sem alterar a mensagem.
- ❌ `git rm arquivo.txt` →                                     #Remove um arquivo e adiciona essa remoção ao commit.
- 🗑️ `git rm --cached arquivo.txt` →                           #Remove o arquivo do controle de versão, mas mantém no diretório local.
- 🔄 `git restore --staged arquivo.txt` →                      #Remove um arquivo do staging, mantendo as mudanças no diretório de trabalho.
- 🧹 `git clean -f` →                                          #Remove arquivos não rastreados do diretório de trabalho.
- 🧹 `git clean -df` →                                        #Remove diretórios e arquivos não rastreados.
- 🔄 `git checkout .` →                                       #Descarta todas as alterações locais nos arquivos rastreados.
- 🚫 `git update-index --skip-worktree arquivo.txt` →         #Ignora temporariamente as alterações em um arquivo rastreado.
- ✅ `git update-index --no-skip-worktree arquivo.txt` →       #Reverte a opção de ignorar alterações em um arquivo rastreado.

## 🔗 Sincronização com Repositórios Remotos

- 🌍 `git remote add origin URL_DO_REPO` →                      #Associa o repositório local a um repositório remoto.
- 🔗 `git remote -v` →                                         #Lista os repositórios remotos configurados.
- 🔄 `git remote get-url origin` →                            #Obtém a URL do repositório remoto.
- 🗑️ `git remote remove origin` →                            #Remove um repositório remoto.
- ✏️ `git remote rename origin novo-nome` →                   #Renomeia um repositório remoto.
- 🔄 `git remote set-branches origin --add branch` →         #Define quais branches são buscadas pelo remoto.
- 📌 `git remote set-head origin main` →                     #Define qual branch é considerada a principal.
- 🔄 `git remote set-url origin https://github.com/USERNAME/REPOSITORIO.git` → #Altera a URL do repositório remoto.
- 🔍 `git remote show origin` →                              #Exibe informações detalhadas sobre um repositório remoto.
- 🔄 `git remote update` →                                   #Atualiza as referências de todos os repositórios remotos.
- 🚀 `git push origin main` →                                #Envia os commits para o repositório remoto.
- 📌 `git push -u origin main` →                            #Define a branch remota como padrão.
- 🔄 `git push --set-upstream origin "nome da branch"` →   #Define a branch atual para acompanhar a branch remota.
- 🗑️ `git push --delete origin nome-da-branch` →           #Exclui uma branch remota.
- 🔄 `git pull origin main` →                               #Atualiza o repositório local com as mudanças remotas.
- 📥 `git fetch` →                                         #Baixa as mudanças do repositório remoto sem mesclá-las.

## ⏪ Reverter Mudanças

- ↩️ `git reset arquivo.txt` →                               #Remove o arquivo do staging, mas mantém as mudanças.
- ⛔ `git reset --hard` →                                   #Descarta todas as mudanças não commitadas.
- 🔙 `git revert HASH_DO_COMMIT` →                         #Cria um novo commit que desfaz um commit anterior.

Esses comandos são essenciais para um uso mais avançado do Git e ajudam a manter o repositório organizado e eficiente! 🚀

