<h3>Git e Github</h3>

##### Termos básicos #####
1. Git: 
Git é um sistema de controle de versão, criado por Linus Torvalds, para desenvolver o Kernel do Linux. 
Com ele você pode fazer e salvar cada alteração em seu projeto e futuramente essas alterações poderão ser consultadas
ou revertidas. É como se você criasse um ponto de restauração no seu sistema, só que no Git realmente funciona!
Com o Git você consegue saber a data, a hora, quem alterou e o que foi alterado. 

2. GitHub (https://github.com/): 
Github é um site que funciona em cima do Git. 
Nele você consegue criar seus projetos e mantê-los online, mas mais do que isso, 
ele também funciona como uma rede social, onde as pessoas conseguem ver seus projetos e contribuir para eles.

3. Commit: 
Um Commit é um pacote de alterações do seu projeto. 
Digamos que você já tenha uma pasta com os arquivos do seu projeto, você acabou de editar um arquivo e 
precisa salvar essas alterações no Git, nesse caso você precisará fazer um Commit.
<br />
Vamos supor que o arquivo alterado tenha sido o “arquivo.txt” que está dentro da pasta textos, nesse caso você executará o seguinte comando:
<pre>git add textos/arquivo.txt</pre>
Feito isso você terá adicionado o arquivo “arquivo.txt” ao Stage, que é onde ele fica antes de ser “comitado”.
Digamos que sua alteração foi somente essa e você quer “comitar” ela para o Git, é só executar o seguinte comando:
<pre>git commit –m “Mensagem descrevendo o que foi alterado”</pre>
Você acaba de criar um commit, um pacote de alterações que contem apenas um arquivo. 
Caso você tenha alterado vários arquivos e deseja incluir todos eles ao mesmo commit, 
troque apenas o caminho do arquivo para “.”, fica assim:
<pre>git add .</pre>
O comando do commit vai continuar o mesmo. 
O que você precisa entender é que ao executar o git add você está adicionando arquivos ao Stage, 
e que ao executar o git commit, tudo que estiver no Stage vai para o HEAD do seu projeto Git local.

Referências: 

* http://www.viniciusdacal.com/pt/iniciante/2015/01/29/o-basico-do-basico-do-git-e-do-github.html 
* http://tableless.com.br/tudo-que-voce-queria-saber-sobre-git-e-github-mas-tinha-vergonha-de-perguntar/

<h4>Passo a passo</h4>
1. Criar uma conta no GitHub (cada aluno deverá ter uma conta)
2. Criar um repositório para o grupo com o nome 'ifpe-pp01-equipeX'
3. Adicionar todos os membros da equipe ao repositório
4. Criar uma pasta local e fazer o clone do projeto
5. Copiar os arquivos já criados para a pasta do projeto
6. Submeter os arquivos para o repositório do github

#### Resumo dos comandos Git ####

<h6>Submeter arquivos para um repositório
<ol>
<li>Direcionar para a pasta onde serão colocados os arquivos do repositório
<pre>cd nome-pasta</pre>
</li>
<li>Clonar o repositório remoto para a pasta local <br />
    <pre>git clone URL</pre></li>
<li>Configurar dados do usuário<br/>
<pre>git config --global user.name SeuNome<br/>
git config --global user.email seuemail-usado-no-github@abc.com <br /> </pre> 
     </li>
<li>Marcar os arquivos novos para commit<br />
    <pre>git add . </pre></li>
<li>Finalizar o pacote de envio dos arquivos marcados<br />
    <pre>git commit -m ‘Mensagem’ </pre></li>
<li>Se existir alguma alteração nova no repositório, será necessário fazer o merge antes:<br />
    <pre>git pull origin master</pre> </li>
<li>Por fim, submeter as suas alterações:<br />
    <pre>git push origin master</pre></li>
</ol>


