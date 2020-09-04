# Curso Básico de Bash Linux com Git e Github para Etec Prof. Camargo Aranha
 
## Comandos Básicos do Git

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
    
8. **Fazer login no Github via git** 
    
        git config --global user.email "[seu email do Github]"
        git config --global user.name "[seu usuário do Github]"

9. **Como permitir tráfego de arquivos com nomes longos** 
    
        git config --system core.longpaths true


10. **Como mudar de branch** 
    
        git checkout [nome da branch]


11. **Como criar uma nova branch (local) e mudar ao mesmo tempo para ela** 
    
        git checkout -b [nome da nova branch]


12. **Como subir a nova branch (local) para nuvem** 
    
        git push --set-upstream origin [nome da nova branch]


13. **COMO FAZER UM SITE COM GITHUB**

        https://blog.paulagrangeiro.com.br/hospedando-sites-gratuitamente-com-o-github-pages-284aa643db14
