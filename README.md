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
