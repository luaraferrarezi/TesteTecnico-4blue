Bug Report - 4blue      
Luara Ferrarezi          
06.03.2026       

Ambiente de teste           
Navegador: Google Chrome           
Sistema operacional: Windows 10          
Tipo de teste: Teste exploratório manual             
Link de Casos de Testes executados: https://docs.google.com/spreadsheets/d/1ahL3nDis4we0AYVkzhwzr09tfTSH1D_vsAJlDOd9O6I/edit?usp=sharing

____
**BUG 01 - C001**

- **Título:** Registro não é realizado ao pressionar a tecla **Enter** no formulário de criação de conta.
  
- **Descrição:** Ao preencher todos os campos corretamente na tela de criação de conta e pressionar a tecla Enter, o sistema não realiza o envio do formulário. O envio só ocorre ao clicar manualmente no botão Criar conta.
  
- **Passos para reproduzir:**          
1. Acessar a tela Criar Conta          
2. Preencher todos os campos com dados válidos
3. Pressionar a tecla Enter no teclado;           

- **Resultado atual:** Nenhuma ação ocorre e o formulário não é enviado.
  
- **Resultado esperado:** Ao pressionar Enter, o sistema deve submeter o formulário, executando a mesma ação do botão Criar conta.
  
- **Severidade:** Média
  
- **Prioridade:** Média          
___                   
**BUG 02 - C002**

- **Título:** Sistema não exibe corretamente múltiplas mensagens de validação quando vários campos estão inválidos
  
- **Descrição:** Ao tentar enviar o formulário de criação de conta com mais de um campo inválido ou vazio, o sistema não exibe corretamente todas as mensagens de validação necessárias para orientar o usuário sobre os erros presentes no formulário.

- **Passos para reproduzir:**       
1. Acessar a tela **Criar Conta**          
2. Preencher o formulário com múltiplos campos inválidos          
3. Clicar no botão Criar conta            

- **Resultado atual:** O sistema exibe apenas uma mensagem de erro e não apresenta claramente todos os campos com problema.
  
- **Resultado esperado:**                
O sistema deve:                       
 Exibir mensagens de validação para todos os campos inválido;                 
 Indicar claramente cada campo que contém erro;                  
 Permitir que o usuário identifique todos os problemas de uma vez;                      
  
- **Severidade:** Média
  
- **Prioridade:** Média
_____      
**BUG 03 - C004**

- **Título:** Sistema permite cadastro mesmo com o campo Nome Completo vazio               
- **Descrição:** Ao tentar realizar o cadastro sem preencher o campo Nome Completo, o sistema permite o envio do formulário e realiza o registro da conta, mesmo sendo um campo que deveria ser obrigatório.
   
- **Passos para reproduzir:**                
1. Acessar a tela Criar Conta              
2. Deixar o campo Nome Completo vazio                
3. Preencher os demais campos com dados válidos                  
4. Clicar no botão Criar conta                   

- **Resultado atual:** O sistema permite o cadastro mesmo com o campo Nome Completo vazio.
  
- **Resultado esperado:**            
O sistema deve:                  
 Bloquear o envio do formulário;                   
 Exibir uma mensagem de validação informando que o campo Nome Completo é obrigatório;                      

- **Severidade:** Alta
  
- **Prioridade:** Alta
  ______________________       
**BUG 04 - C005**

- **Título:** Campo Nome Completo aceita números durante o cadastro
  
- **Descrição:** Ao preencher o campo Nome Completo com números, o sistema permite o envio do formulário e realiza o cadastro normalmente, sem apresentar nenhuma mensagem de validação.
  
- **Passos para reproduzir:**               
1. Acessar a tela Criar Conta              
2. No campo Nome Completo, inserir um valor contendo números                 
    Exemplo: Joao123          
3. Preencher os demais campos com dados válidos              
4. Clicar no botão Criar conta                 

- **Resultado atual:** O sistema aceita o valor inserido contendo números e permite concluir o cadastro.
  
- **Resultado esperado:**             
O sistema deve:               
 Não permitir números no campo Nome Completo;                
 Exibir uma mensagem de validação informando que o nome deve conter apenas letras;                 

- **Severidade:** Média
  
- **Prioridade:** Média
_________________________
**BUG 05 - C006**

- **Título:** Campo Nome Completo permite caracteres especiais no cadastro
  
- **Descrição:** Ao preencher o campo Nome Completo com caracteres especiais, o sistema permite o envio do formulário e realiza o cadastro normalmente, sem apresentar nenhuma validação ou mensagem de erro.
  
- **Passos para reproduzir:**            
1. Acessar a tela Criar Conta            
2. No campo Nome Completo, inserir caracteres especiais             
    Exemplo: João@Silva!       
3. Preencher os demais campos com dados válidos               
4. Clicar no botão Criar conta                 

- **Resultado atual:** O sistema aceita o valor contendo caracteres especiais e permite concluir o cadastro.
  
- **Resultado esperado:**              
O sistema deve:               
 Não permitir caracteres especiais no campo Nome Completo;              
 Exibir uma mensagem de validação informando que o campo deve conter apenas letras;               

- **Severidade:** Média
  
- **Prioridade:** Média
___________________
**BUG 06 - C008**

- **Título:** Campo Telefone aceita número incompleto durante o cadastro
  
- **Descrição:** Ao preencher o campo Telefone com uma quantidade de dígitos menor que o esperado, o sistema permite o envio do formulário e realiza o cadastro normalmente, sem apresentar validação ou mensagem de erro.
  
- **Passos para reproduzir:**           
1. Acessar a tela Criar Conta            
2. Preencher o campo Nome Completo com um valor válido               
3. No campo Telefone, inserir um número incompleto               
    Exemplo: 119876               
4. Preencher os demais campos com dados válidos             
5. Clicar no botão Criar conta                 

- **Resultado atual:** O sistema aceita o telefone com quantidade insuficiente de dígitos e permite concluir o cadastro.
  
- **Resultado esperado:**            
O sistema deve:           
 Validar a quantidade mínima de dígitos do telefone;                   
 Exibir uma mensagem de erro informando que o telefone é inválido ou incompleto;                    
 Bloquear o envio do formulário até que o número seja corrigido;                      

- **Severidade:** Média
  
- **Prioridade:** Média
_____________________________
**BUG 07 - C009**

- **Título:** Campo Telefone permite inserção de letras durante o cadastro
  
- **Descrição:** Ao preencher o campo Telefone com letras, o sistema permite o envio do formulário e realiza o cadastro normalmente, sem apresentar nenhuma validação ou mensagem de erro.
  
- **Passos para reproduzir:**           
1. Acessar a tela Criar Conta             
2. Preencher o campo Nome Completo com um valor válido             
3. No campo Telefone, inserir letras                    
    Exemplo: abcde12345             
4. Preencher os demais campos com dados válidos                   
5. Clicar no botão Criar conta                  

- **Resultado atual:** O sistema aceita letras no campo telefone e permite concluir o cadastro.
  
- **Resultado esperado:**            
O sistema deve:            
 Permitir apenas números no campo telefone;                 
 Exibir uma mensagem de validação informando que o telefone deve conter apenas números;                 
 Bloquear o envio do formulário até que o campo seja corrigido;                

- **Severidade:** Média
  
- **Prioridade:** Média
  ______________________________
**BUG 08 - C011**

- **Título:** Campo Email aceita formato inválido durante o cadastro
  
- **Descrição:** Ao preencher o campo Email com um formato inválido, o sistema permite o envio do formulário e realiza o cadastro normalmente, sem apresentar nenhuma mensagem de validação.
  
- **Passos para reproduzir:**            
1. Acessar a tela Criar Conta              
2. No campo Email, inserir um formato inválido             
    Exemplo: 'usuarioemail.com' ou 'usuario@'              
3. Preencher os demais campos com dados válidos           
4. Clicar no botão Criar conta                

- **Resultado atual:** O sistema aceita o email em formato inválido e permite concluir o cadastro.
  
- **Resultado esperado:**
O sistema deve:            
 Validar o formato do email;              
 Exibir uma mensagem de erro informando que o email é inválido;              
 Bloquear o envio do formulário até que o email esteja em um formato válido;             
    Exemplo: <usuario@email.com>          
  
- **Severidade:** Alta
  
- **Prioridade:** Alta
_____________________________________________
**BUG 09 - C012**

- **Título:** Sistema permite realizar cadastro utilizando email já registrado
  
- **Descrição:** Ao tentar criar uma nova conta utilizando um email que já foi cadastrado anteriormente, o sistema permite concluir o cadastro sem apresentar nenhuma validação ou mensagem de erro.
  
- **Passos para reproduzir:**             
1. Acessar a tela Criar Conta             
2. Realizar um cadastro utilizando um email válido             
3. Após o cadastro ser concluído, voltar para a tela Criar Conta             
4. Tentar realizar um novo cadastro utilizando o mesmo email           
5. Preencher os demais campos com dados válidos             
6. Clicar no botão Criar conta            

- **Resultado atual:** O sistema permite realizar múltiplos cadastros utilizando o mesmo email.
  
- **Resultado esperado:**             
O sistema deve:           
 Verificar se o email já está cadastrado no sistema;              
 Exibir uma mensagem de erro informando que o email já está em uso;             
 Bloquear a criação de uma nova conta com o mesmo email;                     

- **Severidade:** Alta
  
- **Prioridade:** Alta
________________________________________
**BUG 10 - C014**

- **Título:** Campo Senha permite cadastro com menos de 8 caracteres
  
- **Descrição:** Ao preencher o campo Senha com uma quantidade de caracteres menor que o mínimo recomendado (8 caracteres), o sistema permite concluir o cadastro sem apresentar nenhuma validação ou mensagem de erro.
  
- **Passos para reproduzir:**               
1. Acessar a tela Criar Conta              
2. Preencher os campos com dados válidos              
3. No campo Senha, inserir uma senha com menos de 8 caracteres             
    Exemplo: 12345            
4. No campo Confirmar Senha, inserir a mesma senha               
5. Clicar no botão Criar conta               

- **Resultado atual:** O sistema aceita senha com menos de 8 caracteres e permite concluir o cadastro.

- **Resultado esperado:**
O sistema deve:                
 Exigir no mínimo 8 caracteres no campo senha;                 
 Exibir uma mensagem de validação informando que a senha é muito curta;                
 Bloquear o envio do formulário até que a senha atenda ao requisito mínimo;                       

- **Severidade:** Alta

- **Prioridade:** Alta
_____________________________
**BUG 11 - C015**

- **Título:** Campo Senha permite cadastro sem caractere especial

- **Descrição:** Ao preencher o campo Senha sem incluir nenhum caractere especial, o sistema permite concluir o cadastro normalmente, sem apresentar nenhuma validação ou mensagem de erro.

- **Passos para reproduzir:**             
1. Acessar a tela Criar Conta               
2. Preencher os campos com dados válidos:             
3. No campo Senha, inserir uma senha contendo apenas letras e números               
    Exemplo: Senha1234                
4. No campo Confirmar Senha, inserir a mesma senha            
5. Clicar no botão Criar conta                   

- **Resultado atual:** O sistema aceita a senha sem caractere especial e permite concluir o cadastro.

- **Resultado esperado:**             
O sistema deve:               
 Exigir pelo menos um caractere especial na senha;                  
    Exemplos: @ # \$ % ! \*                  
 Exibir uma mensagem de validação informando que a senha precisa conter um caractere especial;              
 Bloquear o envio do formulário até que o requisito seja atendido;                  

- **Severidade:** Média

- **Prioridade:** Média
___________________
**BUG 12 - C016**

- **Título:** Sistema permite cadastro mesmo quando Senha e Confirmar Senha são diferentes
  
- **Descrição:** Ao preencher os campos Senha e Confirmar Senha com valores diferentes, o sistema permite concluir o cadastro sem apresentar nenhuma mensagem de validação.

- **Passos para reproduzir:**             
1. Acessar a tela Criar Conta             
2. Preencher os campos com dados válidos                       
3. No campo Senha, inserir uma senha válida                     
Exemplo: Senha@123                             
4. No campo Confirmar Senha, inserir uma senha diferente                            
Exemplo: Senha@124                           
5. Clicar no botão Criar conta                         

- **Resultado atual:** O sistema permite concluir o cadastro mesmo com os campos Senha e Confirmar Senha contendo valores diferentes.

- **Resultado esperado:**                        
O sistema deve:                    
 Validar se os campos Senha e Confirmar Senha possuem o mesmo valor;                
 Exibir uma mensagem de erro informando que as senhas não coincidem;                         
 Bloquear o envio do formulário até que os valores sejam iguais;                   

- **Severidade:** Alta

- **Prioridade:** Alta
______________________________________
**BUG 13 - C017**

- **Título:** Sistema permite cadastro mesmo com o campo Confirmar Senha vazio
  
- **Descrição:** Ao preencher o campo Senha corretamente e deixar o campo Confirmar Senha vazio, o sistema permite concluir o cadastro sem apresentar mensagem de validação.
  
- **Passos para reproduzir:**                 
1. Acessar a tela Criar Conta              
2. Preencher os campos com dados válidos                  
3. No campo Senha, inserir uma senha válida                   
    Exemplo: Senha@123                  
4. Deixar o campo Confirmar Senha vazio                  
5. Clicar no botão Criar conta                           

- **Resultado atual:** O sistema permite concluir o cadastro mesmo com o campo Confirmar Senha vazio
.
- **Resultado esperado:**                  
O sistema deve:                      
 Exigir o preenchimento do campo Confirmar Senha;                        
 Exibir uma mensagem de validação informando que o campo é obrigatório;                 
 Bloquear o envio do formulário até que o campo seja preenchido corretamente;                     

- **Severidade:** Alta
  
- **Prioridade:** Alta
__________________________________________________
**BUG 14 - C027**

- **Título:** Sistema permite envio do login com o campo Senha vazio
  
- **Descrição:** Ao tentar realizar login preenchendo apenas o campo Email e deixando o campo Senha vazio, o sistema permite o envio do formulário sem apresentar validação informando que o campo é obrigatório.
  
- **Passos para reproduzir:**          
1. Acessar a tela **Login**                 
2. Inserir um **email válido** no campo Email                
3. Deixar o campo **Senha** vazio              
4. Clicar no botão **Entrar**             

- **Resultado atual:** O sistema permite o envio do formulário mesmo com o campo senha vazio.
  
- **Resultado esperado:**
O sistema deve:            
 Validar que o campo Senha é obrigatório;                  
 Exibir uma mensagem de erro informando que a senha deve ser preenchida;                     
 Bloquear a tentativa de login até que o campo seja preenchido;                            

- **Severidade:** Média
  
- **Prioridade:** Alta
______________________________________
**BUG 15 - C029**

- **Título:** Tecla Enter não envia o formulário de login
  
- **Descrição:** Ao preencher os campos de Email e Senha na tela de login e pressionar a tecla Enter, o sistema não realiza o envio do formulário. O login só ocorre ao clicar manualmente no botão Entrar.
  
- **Passos para reproduzir:**                      
1. Acessar a tela Login                      
2. Preencher o campo Email com um email válido                            
3. Preencher o campo Senha com uma senha válida                 
4. Pressionar a tecla Enter no teclado                              

- **Resultado atual:** Nada acontece e o login não é realizado ao pressionar Enter.
  
- **Resultado esperado:**              
O sistema deve:                      
 Permitir o envio do formulário ao pressionar a tecla Enter;                       
 Realizar o login da mesma forma que ao clicar no botão Entrar;                          

- **Severidade:** Baixa
  
- **Prioridade:** Baixa
______________________________________
**BUG 16 - C035**

- **Título:** Usuário consegue acessar a tela de sucesso diretamente pela URL sem realizar cadastro
  
- **Descrição:** Foi identificado que a tela de sucesso pode ser acessada diretamente ao inserir sua URL no navegador, mesmo sem ter realizado o processo de cadastro ou login no sistema.
Isso permite que qualquer usuário visualize a página sem passar pelo fluxo correto da aplicação.

- **Passos para reproduzir:**                           
1. Copiar a URL da tela de sucesso             
2. Abrir uma nova aba do navegador                      
3. Colar a URL diretamente na barra de endereço                    
4. Pressionar Enter                         
 
- **Resultado atual:** A tela de sucesso é exibida normalmente, mesmo sem o usuário ter realizado cadastro ou login no sistema.
  
- **Resultado esperado:**                    
**O sistema deve:**                       
 Verificar se o usuário passou pelo fluxo correto de cadastro;                
 Bloquear o acesso direto à página;                 
 Redirecionar o usuário para: Tela de Login, ou Tela de Criação de Conta;                  

- **Severidade:** Alta
  
- **Prioridade:** Alta
  _________________________________________________
# **Quais 2 bugs você corrigiria primeiro e por quê?**

1\. Sistema permite login com campo senha vazio

**Motivo da priorização:** Esse bug possui alta severidade, pois afeta diretamente o processo de autenticação do sistema

Permitir que o formulário de login seja enviado sem preencher o campo senha pode indicar falha na validação de entrada de dados, o que pode comprometer: a segurança do sistema, o controle de acesso, a confiabilidade do processo de autenticação. Como o login é uma funcionalidade crítica da aplicação, esse problema deveria ser corrigido imediatamente
***
2\. Sistema permite cadastro com email já registrado

**Motivo da priorização:** Permitir o cadastro de múltiplas contas utilizando o mesmo email pode gerar problemas de: duplicidade de contas, inconsistência de dados no sistema, problemas em recuperação de senha, confusão na identificação de usuários.  
Como o email geralmente é utilizado como identificador único de conta, essa validação é essencial para manter a integridade da base de usuários.
__________________________
# **Sugestões de melhorias para as telas**

1\. Implementar validações mais robustas nos formulários

Alguns campos permitem inserção de dados inválidos. Seria recomendado implementar validações como:             

 Nome completo não aceitar números ou caracteres especiais            
 Telefone aceitar apenas números e validar quantidade de dígitos           
 Email validar formato corretamente                
 Senha exigir critérios mínimos de segurança               
***
2\. Melhorar feedback visual de erros

O sistema poderia apresentar mensagens de validação mais claras e imediatas, informando ao usuário exatamente qual campo está incorreto e como corrigir. Isso melhora significativamente a experiência do usuário.
***
3\. Permitir envio de formulários pressionando a tecla Enter

Permitir o envio de formulários através da tecla Enter melhora a usabilidade e acessibilidade, seguindo padrões comuns de aplicações web.
***
4\. Indicador de força da senha

Durante o processo de criação de conta, seria interessante implementar um indicador de força da senha, exibido abaixo do campo de senha enquanto o usuário digita. Esse indicador poderia informar visualmente se a senha é fraca, média ou forte.

Além disso, também poderia mostrar os requisitos necessários para uma senha válida, como por exemplo:                   

 mínimo de 8 caracteres           
 pelo menos uma letra maiúscula           
 pelo menos um número               
 pelo menos um caractere especial             

À medida que o usuário digita a senha, os requisitos poderiam ser marcados como atendidos, ajudando o usuário a entender facilmente o que ainda precisa ser ajustado.
