# Script_backup-shell-Postgres
Script para fazer backup

Comandos necessarios:

#!/bin/bash

#senha PGADMIN

export PGPASSWORD="170216"

#código

pg_dump -U postgres -h localhost -O -o -b -F c faculdade > /home/morgenstern/Documentos/morgenstern.backup

#mensagem

echo echo "backup realizado!!!."

exit 



#!/bin/bash

#senha PGADMIN

export PGPASSWORD="170216"

#código

pg_restore -U postgres -h localhost -d faculdade2 /home/morgenstern/Documentos/morgenstern.backup

#mensagem

echo echo "Seu backup foi restaurado com sucesso."

exit 
