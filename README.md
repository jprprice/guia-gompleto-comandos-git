<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="Guia_Completo_de_Comandos_Git__0"></a>Guia Completo de Comandos Git 🚀</h1>
<h2 class="code-line" data-line-start=2 data-line-end=3 ><a id="_Configurao_Inicial_do_Git_2"></a>🔧 Configuração Inicial do Git</h2>
<ul>
<li class="has-line-data" data-line-start="4" data-line-end="5">📝 <code>git config --global user.name &quot;Seu Nome&quot;</code> →                   #Define o nome do usuário.</li>
<li class="has-line-data" data-line-start="5" data-line-end="6">📧 <code>git config --global user.email &quot;seuemail@example.com&quot;</code> →      #Define o e-mail do usuário.</li>
<li class="has-line-data" data-line-start="6" data-line-end="7">⚙️ <code>git config --list</code> →                                          #Exibe as configurações do Git.</li>
<li class="has-line-data" data-line-start="7" data-line-end="8">🌿 <code>git config --global init.defaultBranch &lt;name&gt;</code> →              #Define o nome padrão da branch inicial ao criar um novo repositório.</li>
<li class="has-line-data" data-line-start="8" data-line-end="9">✏️ <code>git config --global core.editor &quot;editor&quot;</code> →                   #Define o editor de texto padrão para o Git.</li>
<li class="has-line-data" data-line-start="9" data-line-end="11">📜 <code>git config --global core.pager cat</code> →                         #Define o pager padrão do Git para exibir saída diretamente no terminal.</li>
</ul>
<h2 class="code-line" data-line-start=11 data-line-end=12 ><a id="_Inicializao_e_Clonagem_11"></a>📂 Inicialização e Clonagem</h2>
<ul>
<li class="has-line-data" data-line-start="13" data-line-end="14">🆕 <code>git init</code> →                                                   #Inicializa um repositório Git na pasta atual.</li>
<li class="has-line-data" data-line-start="14" data-line-end="16">🔄 <code>git clone URL_DO_REPO</code> →                                      #Clona um repositório remoto para o computador.</li>
</ul>
<h2 class="code-line" data-line-start=16 data-line-end=17 ><a id="_Status_e_Histrico_16"></a>📜 Status e Histórico</h2>
<ul>
<li class="has-line-data" data-line-start="18" data-line-end="19">🔍 <code>git status</code> →                                                 #Mostra o status dos arquivos (modificados, adicionados, etc.).</li>
<li class="has-line-data" data-line-start="19" data-line-end="20">📜 <code>git log</code> →                                                    #Exibe o histórico de commits.</li>
<li class="has-line-data" data-line-start="20" data-line-end="21">📊 <code>git log --oneline --graph</code> →                                  #Exibe um histórico resumido e visual.</li>
<li class="has-line-data" data-line-start="21" data-line-end="22">📌 <code>git log --oneline</code> →                                          #Mostra o histórico de commits em uma única linha por commit.</li>
<li class="has-line-data" data-line-start="22" data-line-end="23">🧐 <code>git log -p</code> →                                                 #Exibe o histórico de commits com as diferenças de cada mudança.</li>
<li class="has-line-data" data-line-start="23" data-line-end="24">📊 <code>git log --stat</code> →                                             #Mostra estatísticas das alterações em cada commit.</li>
<li class="has-line-data" data-line-start="24" data-line-end="25">🔍 <code>git diff</code> →                                                   #Exibe as diferenças entre os arquivos modificados e o último commit.</li>
<li class="has-line-data" data-line-start="25" data-line-end="27">🔄 <code>git diff --cached</code> →                                          #Exibe as diferenças dos arquivos adicionados ao staging em relação ao último commit.</li>
</ul>
<h2 class="code-line" data-line-start=27 data-line-end=28 ><a id="_Trabalhando_com_Arquivos_27"></a>🛠️ Trabalhando com Arquivos</h2>
<ul>
<li class="has-line-data" data-line-start="29" data-line-end="30">➕ <code>git add arquivo.txt</code> →                                        #Adiciona um arquivo específico ao staging.</li>
<li class="has-line-data" data-line-start="30" data-line-end="31">📂 <code>git add .</code> →                                                  #Adiciona <strong>todos os arquivos</strong> modificados ao staging.</li>
<li class="has-line-data" data-line-start="31" data-line-end="32">✅ <code>git commit -m &quot;Mensagem do commit&quot;</code> →                         #Confirma as mudanças adicionadas.</li>
<li class="has-line-data" data-line-start="32" data-line-end="33">✏️ <code>git commit --amend</code> →                                         #Modifica o último commit.</li>
<li class="has-line-data" data-line-start="33" data-line-end="34">🔄 <code>git commit --amend --no-edit</code> →                               #Modifica o último commit sem alterar a mensagem.</li>
<li class="has-line-data" data-line-start="34" data-line-end="35">❌ <code>git rm arquivo.txt</code> →                                         #Remove um arquivo e adiciona essa remoção ao commit.</li>
<li class="has-line-data" data-line-start="35" data-line-end="36">🗑️ <code>git rm --cached arquivo.txt</code> →                                #Remove o arquivo do controle de versão, mas mantém no diretório local.</li>
<li class="has-line-data" data-line-start="36" data-line-end="37">🔄 <code>git restore --staged arquivo.txt</code> →                           #Remove um arquivo do staging, mantendo as mudanças no diretório de trabalho.</li>
<li class="has-line-data" data-line-start="37" data-line-end="38">🧹 <code>git clean -f</code> →                                               #Remove arquivos não rastreados do diretório de trabalho.</li>
<li class="has-line-data" data-line-start="38" data-line-end="39">🧹 <code>git clean -df</code> →                                              #Remove diretórios e arquivos não rastreados.</li>
<li class="has-line-data" data-line-start="39" data-line-end="40">🔄 <code>git checkout .</code> →                                             #Descarta todas as alterações locais nos arquivos rastreados.</li>
<li class="has-line-data" data-line-start="40" data-line-end="41">🚫 <code>git update-index --skip-worktree arquivo.txt</code> →               #Ignora temporariamente as alterações em um arquivo rastreado.</li>
<li class="has-line-data" data-line-start="41" data-line-end="43">✅ <code>git update-index --no-skip-worktree arquivo.txt</code> →            #Reverte a opção de ignorar alterações em um arquivo rastreado.</li>
</ul>
<h2 class="code-line" data-line-start=43 data-line-end=44 ><a id="_Sincronizao_com_Repositrios_Remotos_43"></a>🔗 Sincronização com Repositórios Remotos</h2>
<ul>
<li class="has-line-data" data-line-start="45" data-line-end="46">🌍 <code>git remote add origin URL_DO_REPO</code> →                          #Associa o repositório local a um repositório remoto.</li>
<li class="has-line-data" data-line-start="46" data-line-end="47">🔗 <code>git remote -v</code> →                                              #Lista os repositórios remotos configurados.</li>
<li class="has-line-data" data-line-start="47" data-line-end="48">🔄 <code>git remote get-url origin</code> →                                  #Obtém a URL do repositório remoto.</li>
<li class="has-line-data" data-line-start="48" data-line-end="49">🗑️ <code>git remote remove origin</code> →                                   #Remove um repositório remoto.</li>
<li class="has-line-data" data-line-start="49" data-line-end="50">✏️ <code>git remote rename origin novo-nome</code> →                         #Renomeia um repositório remoto.</li>
<li class="has-line-data" data-line-start="50" data-line-end="51">🔄 <code>git remote set-branches origin --add branch</code> →                #Define quais branches são buscadas pelo remoto.</li>
<li class="has-line-data" data-line-start="51" data-line-end="52">📌 <code>git remote set-head origin main</code> →                            #Define qual branch é considerada a principal.</li>
<li class="has-line-data" data-line-start="52" data-line-end="53">🔄 <code>git remote set-url origin NOVA_URL</code> →                         #Altera a URL do repositório remoto.</li>
<li class="has-line-data" data-line-start="53" data-line-end="54">🔍 <code>git remote show origin</code> →                                     #Exibe informações detalhadas sobre um repositório remoto.</li>
<li class="has-line-data" data-line-start="54" data-line-end="55">🔄 <code>git remote update</code> →                                          #Atualiza as referências de todos os repositórios remotos.</li>
<li class="has-line-data" data-line-start="55" data-line-end="56">🚀 <code>git push origin main</code> →                                       #Envia os commits para o repositório remoto.</li>
<li class="has-line-data" data-line-start="56" data-line-end="57">📌 <code>git push -u origin main</code> →                                    #Define a branch remota como padrão.</li>
<li class="has-line-data" data-line-start="57" data-line-end="58">🔄 <code>git push --set-upstream origin &quot;nome da branch&quot;</code> →            #Define a branch atual para acompanhar a branch remota.</li>
<li class="has-line-data" data-line-start="58" data-line-end="59">🗑️ <code>git push --delete origin nome-da-branch</code> →                    #Exclui uma branch remota.</li>
<li class="has-line-data" data-line-start="59" data-line-end="60">🔄 <code>git pull origin main</code> →                                       #Atualiza o repositório local com as mudanças remotas.</li>
<li class="has-line-data" data-line-start="60" data-line-end="62">📥 <code>git fetch</code> →                                                  #Baixa as mudanças do repositório remoto sem mesclá-las.</li>
</ul>
<h2 class="code-line" data-line-start=62 data-line-end=63 ><a id="_Branches_Ramificaes_62"></a>🌱 Branches (Ramificações)</h2>
<ul>
<li class="has-line-data" data-line-start="64" data-line-end="65">🌳 <code>git branch</code> →                                                 #Lista as branches existentes.</li>
<li class="has-line-data" data-line-start="65" data-line-end="66">🌱 <code>git branch nome-da-branch</code> →                                  #Cria uma nova branch.</li>
<li class="has-line-data" data-line-start="66" data-line-end="67">🔄 <code>git checkout nome-da-branch</code> →                                #Muda para outra branch.</li>
<li class="has-line-data" data-line-start="67" data-line-end="68">🆕 <code>git checkout -b nova-branch</code> →                                #Cria e muda para uma nova branch.</li>
<li class="has-line-data" data-line-start="68" data-line-end="69">🔀 <code>git merge nome-da-branch</code> →                                   #Mescla uma branch com a atual.</li>
<li class="has-line-data" data-line-start="69" data-line-end="70">🗑️ <code>git branch -d nome-da-branch</code> →                               #Deleta uma branch local.</li>
<li class="has-line-data" data-line-start="70" data-line-end="71">🗑️ <code>git branch -D nome-da-branch</code> →                               #Força a exclusão de uma branch local.</li>
<li class="has-line-data" data-line-start="71" data-line-end="72">✏️ <code>git branch -m &lt;name&gt;</code> →                                       #Renomeia a branch atual para um novo nome.</li>
<li class="has-line-data" data-line-start="72" data-line-end="73">🔄 <code>git branch -r</code> →                                              #Lista as branches remotas.</li>
<li class="has-line-data" data-line-start="73" data-line-end="74">📌 <code>git branch -a</code> →                                              #Lista todas as branches locais e remotas.</li>
<li class="has-line-data" data-line-start="74" data-line-end="75">🔗 <code>git branch HEAD</code> →                                            #Mostra para qual commit HEAD está apontando.</li>
<li class="has-line-data" data-line-start="75" data-line-end="76">🏷️ <code>git branch master</code> →                                          #Mostra se a branch master existe no repositório.</li>
<li class="has-line-data" data-line-start="76" data-line-end="77">🌍 <code>git branch origin/HEAD</code> →                                     #Mostra para qual branch HEAD do remoto está apontando.</li>
<li class="has-line-data" data-line-start="77" data-line-end="79">🔄 <code>git branch origin/master</code> →                                   #Exibe a referência para a branch master no repositório remoto.</li>
</ul>
<h2 class="code-line" data-line-start=79 data-line-end=80 ><a id="_Reverter_Mudanas_79"></a>⏪ Reverter Mudanças</h2>
<ul>
<li class="has-line-data" data-line-start="81" data-line-end="82">↩️ <code>git reset arquivo.txt</code> →                                      #Remove o arquivo do staging, mas mantém as mudanças.</li>
<li class="has-line-data" data-line-start="82" data-line-end="83">⛔ <code>git reset --hard</code> →                                           #Descarta todas as mudanças não commitadas.</li>
<li class="has-line-data" data-line-start="83" data-line-end="85">🔙 <code>git revert HASH_DO_COMMIT</code> →                                  #Cria um novo commit que desfaz um commit anterior.</li>
</ul>
<p class="has-line-data" data-line-start="85" data-line-end="86">Esses comandos são essenciais para um uso mais avançado do Git e ajudam a manter o repositório organizado e eficiente! 🚀</p>