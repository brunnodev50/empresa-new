# Quem pode acessar o usuarios/cadastrar.php
usuario perfil admin, master, gestor, tecnico e dev

# Quem pode editar e desativar o usuarios usuarios/cadastrar.php
master e gestor

# chamados/lista.php
admin: Acessa todos os chamados, pode criar, editar e encerrar qualquer um.
supervisor: Pode abrir, gerenciar, atribuir chamados a técnicos e atualizar o status.
tecnico: Pode abrir (se permitido), atender os que foram atribuídos a ele, atualizar status, inserir observações/fotos e consultar seu próprio histórico.
cliente: Pode abrir, acompanhar o status dos seus próprios chamados e inserir informações adicionais. Não vê chamados de outros.
# chamados/ver.php
texto em log.
anexo de aquivos: imagens, pdf e video.

# Esquecimento/ Reset senha 

esqueceu_senha.php (onde o usuário digita o e-mail).

redefinir_senha.php (onde o usuário cria a nova senha).

ALTER TABLE usuarios 
ADD COLUMN reset_token VARCHAR(255) NULL DEFAULT NULL, 
ADD COLUMN reset_expires DATETIME NULL DEFAULT NULL;
<img width="1717" height="814" alt="image" src="https://github.com/user-attachments/assets/b02eaa9e-be4a-488a-afdd-f4813a144518" />
<img width="1275" height="760" alt="image" src="https://github.com/user-attachments/assets/f5c36053-1415-4bde-bd58-c88837b5afac" />
<img width="859" height="790" alt="image" src="https://github.com/user-attachments/assets/326768a5-7bda-4bf1-84ce-561b2c1533ad" />
<img width="962" height="458" alt="image" src="https://github.com/user-attachments/assets/baf93013-58b9-4053-91c8-40dc91071616" />
<img width="1074" height="720" alt="image" src="https://github.com/user-attachments/assets/e6346eb0-f5e7-4aaf-9fda-81b23927e07f" />
<img width="935" height="653" alt="image" src="https://github.com/user-attachments/assets/e49cd28a-3dc2-4fe4-a545-0e3765dc0df2" />

# usuarios/cadastrar.php
Cadastramento de user.

# usuarios/perfil.php

