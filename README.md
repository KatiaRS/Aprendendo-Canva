# GIT Tutorial Para Iniciantes
### Passo a Passo

O objetivo desse GIT tutorial é apresentar tudo o que você precisa para começar a usá-lo.

Primeiro de tudo, entenda que o GIT é um sistema de controle de versão, também conhecido pela sigla VCS –  version control system.

Os VCS são uma ótima forma de otimizar o trabalho ao analisar as alterações feitas em um código de projeto compartilhado, além de ser um componente fundamental do sistema de gerenciamento de configuração de software que cuida das mudanças que precisam ser feitas em um projeto.

As alterações/revisões/ atualizações feitas são identificáveis ​​através de códigos de letra ou números. Informações como data e a identidade do autor da alteração também são mantidas.

Neste tutorial, vamos focar no GIT, um dos sistemas de controle de versão mais usados no mundo.

 
## O que é GIT?

Em 2005, Linus Torvalds (o homem conhecido por criar o núcleo, ou kernel, do SO Linux) desenvolveu o GIT, que desde então tem sido ativamente mantido por Junio ​​Hamano, um engenheiro de software japonês.

Atualmente, o GIT é um dos mais famosos sistemas de controle de versão de código aberto e milhões de projetos no mundo inteiro o utilizam para seu controle de versão (incluindo projetos comerciais e de código aberto).

O Git é totalmente grátis e pode ser instalado em Mac, Linux, Windows e Solaris diretamente do site oficial. Algumas das características essenciais do GIT são:

Um sistema de controle de versão distribuído, o GIT segue uma abordagem peer to peer, contrário de outros como o Subversion (SVN) que segue um modelo baseado em cliente-servidor.
GIT permite aos desenvolvedores ter uma infinidade de ramos de código completamente independente. Criação, exclusão e fusão desses ramos é simples e não leva tempo.
No GIT, todas as operações são atômicas. Isso significa que uma ação pode ter sucesso ou falhar (sem fazer nenhuma alteração). Isso é importante porque em alguns sistemas de controle de versão (como o CVS) onde as operações não são atômicas, se uma operação de repositório é suspensa, ela pode deixar o repositório em um estado instável.
No GIT, tudo é armazenado dentro da pasta .git. Isso não é o mesmo em outros VCS como SVN e CVS onde os metadadados de arquivos são armazenados em pastas ocultas (por exemplo, .cvs, .svn, etc.)
GIT usa um modelo de dados que ajuda a garantir a integridade criptográfica de qualquer coisa presente dentro de um repositório. Cada vez que um arquivo é adicionado ou um commit é feito, suas somas de verificação são geradas. Da mesma forma, eles são recuperados através de suas somas de verificação também.
Outra característica presente no GIT é sua área de teste ou índice. Na área de preparação, os desenvolvedores podem formatar commits e receber feedback ​​antes de aplicá-los.

O GIT é consideravelmente simples de usar. Para começar, você pode criar um repositório ou conferir um já existente. Após a instalação, um simples git-init irá deixar tudo pronto. Da mesma maneira, o comando git clone pode criar uma cópia de um repositório local para um usuário.


## 1º Passo – Instalar o GIT em Sistemas Diferentes

Nos parágrafos abaixo vamos ensinar a maneira mais simples de instalar o Git em diversos sistemas operacionais:

Instalar o GIT no Windows:
Instalar o GIT no Windows é tão simples como baixar um instalador e executá-lo. Execute os seguintes passos para instalar o GIT no Windows:

Acesse o site oficial e faça o download do instalador do GIT para Windows.
Depois de baixado, clique duas vezes no arquivo para iniciar o assistente de instalação. Basta seguir as instruções na tela, clicando em Next. Ao término, clique em Finish para concluir com êxito a instalação.

git janela de instalação
Abra o prompt de comando e digite os seguintes comandos no terminal:
git config --global user.name "João Silva"
git config --global user.email "exemplo@seuemail.com.br"

Nota: Lembre de substituir João Silva e exemplo@seuemail.com.br com seus dados. Qualquer commit criado posteriormente será associado à esses dados.

GIT instalado no Windows com sucesso!

### Instalar o GIT no MacOS:

Existem muitas maneiras de instalar o GIT em um Mac. Inclusive, há uma chance de que o GIT já esteja no seu computador se você tiver o XCode instalado. Execute o seguinte comando no terminal para verificar:

git --version
Se você obtiver uma resposta como git version 2.7.0 (Apple Git-66), então você está com sorte. Caso você não tenha resposta, execute os seguintes passos:

Visite este site e faça o download do instalador mais recente para Mac.
Siga as instruções na tela e conclua a instalação.
git instalação no macos
Tente novamente o comando git --version para confirmar se a instalação foi bem sucedida.
Execute os seguintes comandos no terminal para configurar seu e-mail e nome de usuário que serão associados à sua conta GIT:
git config --global user.name "João Silva"
git config --global user.email "exemplo@seuemail.com.br"
Nota: Lembre-se de substituir João Silva e exemplo@seuemail.com.br com seus dados. Qualquer commit criado posteriormente será associado à esses dados.

### Instalar o GIT no Linux:

Se você é um usuário Linux, então deve estar acostumado com instalar programas e pacotes em seu computador usando comandos de instalação apt-get ou yum. Instalar o GIT não é diferente:

### Para usuários Debian/Ubuntu (apt-get):

Abra o terminal e execute os seguintes comandos:
sudo apt-get update 
sudo apt-get install git
Verifique se a instalação ocorreu com sucesso usando git --version.
Execute os seguintes comandos no terminal para configurar seu e-mail e nome de usuário que serão associados à sua conta GIT:
git config --global user.name "João Silva" 
git config --global user.email "exemplo@seuemail.com.br"
Nota: Lembre-se de substituir João Silva e exemplo@seuemail.com.br com seus dados. Qualquer commit criado posteriormente será associado à esses dados.


Fedora (yum/dnf):
Você pode baixar pacotes do GIT usando yum e dnf.

Abra o terminal e execute os seguintes comandos:
sudo dnf install git
sudo yum install git
Verifique se a instalação ocorreu com sucesso usando git --version.
Execute os seguintes comandos no terminal para configurar seu e-mail e nome de usuário que serão associados à sua conta GIT:
git config --global user.name "João Silva"
git config --global user.email "exemplo@seuemail.com.br"
Nota: Lembre-se de substituir João Silva e exemplo@seuemail.com.br com seus dados. Qualquer commit criado posteriormente será associado à esses dados.

##2º Passo – Como Usar o GIT

Agora que o GIT está instalado e configurado no seu dispositivo, vamos explorar os conceitos básicos do GIT e como começar a usar o GIT.
