# Boas práticas para IPtables

1. **Princípio do Deny All**:
Utilize uma política padrão de DENY para bloquear tudo e garantir que nenhum tráfego seja permitido a menos que especificamente permitido pelas regras.

2. **Regras específicas**:
Defina regras específicas para permitir apenas que serviços e portas necessárias para o funcionamento do servidor.

3. **Ordem das regras**:
Regras são processadas de **cima para baixo**, então coloque as regras mais restritivas no início e regras mais permissivas no final.
