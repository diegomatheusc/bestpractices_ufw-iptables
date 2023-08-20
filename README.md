# IPtables

1. **Princípio do Deny All**:
Utilize uma política padrão de DENY para bloquear tudo e garantir que nenhum tráfego seja permitido a menos que especificamente permitido pelas regras.

2. **Regras específicas**:
Defina regras específicas para permitir apenas que serviços e portas necessárias para o funcionamento do servidor.

3. **Ordem das regras**:
Regras são processadas de **cima para baixo**, então coloque as regras mais restritivas no início e regras mais permissivas no final.

4. **Loopback**:
É necessário permitir o tráfego na interface de rede loopback (lo), pois muitos serviços internos dependem disso.

5. **Conexões estabelecidades e relacionadas**:
Permita o tráfego de conexões já estabelecidas e conexões relacionadas ao tráfego permitido para que as respostas sejam permitidas.

6. **Limite tentativas de conexão**:
Para isso, utilize a opção *limit* para isso e evitar um ataque de força bruta ou DDoS.

```
--limite
```

7. **Evite o Port Knocking**.
   
8. **Log de Regras Descartadas**:
Considere o registro de pacotes descartados para fins de auditoria e resolução de problemas.

# UFW:

1. **Enable e Disable**:
Use o UFW para ativar e desativar o firewall facilmente, mas lembre-se de habilitá-lo apenas depois de ter configurado as regras corretas.

2. **Configuração básica**:

