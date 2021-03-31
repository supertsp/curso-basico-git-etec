# Curso Básico de Bash Linux com Git e Github

1. **Copiar um repositório online**    
    
        git clone [url do repositório]


2. **Adicionar mudanças na branch (timeline)**    
    
        git add .
    
    
3. **Verificar mudanças no repositório local**    
    
        git status


4. **Fazer um comentário sobre as mudanças**    
    
        git commit -m "[comentário]"

    
5. **Fazer upload das atualizações locais para nuvem**     
    
        git push
    
6. **Fazer download das atualizações da nuvem para máquina local**    
    
        git pull
    
7. **Baixar apenas o status das atualizações da nuvem**    

        git fetch
        git status
    
8. **Como alterar variáveis do Git para fazer login no Github** 
    
        git config --global user.nickname "[seu usuário do Github]"
        git config --global user.email "[seu email do Github]"
        git config --global user.name "[seu nome]"


9. **Como mudar de branch** 
    
        git checkout [nome da branch]


10. **Como criar uma nova branch (local) e mudar ao mesmo tempo para ela** 
    
        git checkout -b [nome da nova branch]


11. **Como subir a nova branch (local) para nuvem** 
    
        git push --set-upstream origin [nome da nova branch]


12. **Como fazer e publicar um site no Github**

        https://blog.paulagrangeiro.com.br/hospedando-sites-gratuitamente-com-o-github-pages-284aa643db14


13. **Como permitir tráfego de arquivos com nomes longos** 
    
        git config --system core.longpaths true


14. **Como permitir uso do git em redes sem SSL ou com problemas de certificado** 
    
        git config http.sslVerify "false"


15. **Como descobrir as modificações/contribuições de cada usuário em um determinado arquivo** 
    
        git blame -W -C -M [nome do arquivo]
    
    ou
        
        git blame -W -C -M [nome do arquivo] > [endereço + nome do arquivo a ser criado]


16. **Como fazer Merge (fusão) entre 2 branches** 
    
        git merge [nome da brach que está pegando]
    
    ou
        
        git merge --no-ff [nome da brach que está pegando]


17. **Como criar um Tag (marcador) nos commits para indicar versões (releases) de código** 
    
        git tag -a [versao] -m "Release [versao]"

        git push --tags


18. **Como mudar as alterações de código de uma branch para outra** 
    
        (branch-01) $ git stash

        (branch-01) $ git checkout branch-02
        
        (branch-02) $ git stash pop 




19. **Quando uma Senha é alterada na Nuvem, Como alterar no Git Local [Windows]?** 
    
        Abra: Painel de Controle\Contas de Usuário\Gerenciador de Credenciais
        Depois: Selecione "Credenciais Windows", selecione qual credencial deseja e clique em "Editar"
        dsfsf
        
  ou 
       
        git config --list                               --> para ver as configurações
        git remote set-url origin https://[nova URL]    --> para alterar a url de conexão atual



