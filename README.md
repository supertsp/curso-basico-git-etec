# Curso Básico de Bash Linux com Git e Github

1. **Copiar um repositório online**    
    
        git clone [url do repositório]


2. **Adicionar mudanças na branch (timeline)**    
    
        git add .
    
    
3. **Verificar mudanças no repositório local**    
    
        git status


4. **Fazer um comentário sobre as mudanças**    
    
        git commit -m "[comentário]"


5. **Como alterar um comentário recente**    
    
        git commit --amend
        
    
6. **Fazer upload das atualizações locais para nuvem**     
    
        git push
    
7. **Fazer download das atualizações da nuvem para máquina local**    
    
        git pull
    
8. **Baixar apenas o status das atualizações da nuvem**    

        git fetch
        git status
    
9. **Como alterar variáveis do Git para fazer login no Github** 
    
        git config --global user.nickname "[seu usuário do Github]"
        git config --global user.email "[seu email do Github]"
        git config --global user.name "[seu nome]"


10. **Como mudar de branch** 
    
        git checkout [nome da branch]


11. **Como criar uma nova branch (local) e mudar ao mesmo tempo para ela** 
    
        git checkout -b [nome da nova branch]


12. **Como subir a nova branch (local) para nuvem** 
    
        git push --set-upstream origin [nome da nova branch]


13. **Como fazer e publicar um site no Github**

        https://blog.paulagrangeiro.com.br/hospedando-sites-gratuitamente-com-o-github-pages-284aa643db14


14. **Como permitir tráfego de arquivos com nomes longos** 
    
        git config --system core.longpaths true


15. **Como permitir uso do git em redes sem SSL ou com problemas de certificado** 
    
        git config http.sslVerify "false"
        
    ou
        
        git config --global http.sslVerify false


16. **Como descobrir as modificações/contribuições de cada usuário em um determinado arquivo** 
    
        git blame -W -C -M [nome do arquivo]
    
    ou
        
        git blame -W -C -M [nome do arquivo] > [endereço + nome do arquivo a ser criado]


17. **Como fazer Merge (fusão) entre 2 branches** 
    
        git merge [nome da brach que está pegando]
    
    ou
        
        git merge --no-ff [nome da brach que está pegando]


18. **Como trabalhar com Tag (marcadores) para destacar Releases de código** 

    Criando uma tag  

        git tag -a [versao] -m "Release [versao]"

        git push --tags
        
    Listando Tags locais
       
        git tag 
        
    Excluindo uma Tag local
       
        git tag -d [nome da tag]



19. **Como mudar as alterações de código de uma branch para outra** 
    
        (branch-01) $ git stash

        (branch-01) $ git checkout branch-02
        
        (branch-02) $ git stash pop 




20. **Quando uma Senha é alterada na Nuvem, Como alterar no Git Local [Windows]?** 
    
        Abra: Painel de Controle\Contas de Usuário\Gerenciador de Credenciais
        Depois: Selecione "Credenciais Windows", selecione qual credencial deseja e clique em "Editar"
        
    ou 
       
        git config --list                               --> para ver as configurações
        git remote set-url origin https://[nova URL]    --> para alterar a url de conexão atual



