## O que é a Walletly?

Walletly é uma plataforma de gestão financeira pessoal focada em:

- Importação de dados financeiros via CSV    
- Organização automática e manual de transações    
- Cálculo de previsibilidade financeira  (CPF)  
- Geração de insights com IA    
- Visualização simplificada via dashboards    

O objetivo atual não é apenas produto, mas também evolução arquitetural sólida.

---

# Como ela funciona (modelo atual)

## Fluxo principal

1. Usuário cria conta    
2. Usuário importa CSV com suas transações    
3. O sistema:    
    - Publica evento no RabbitMQ        
    - Microsserviço consome o evento        
    - Processa o CSV        
    - Categoriza (IA)        
    - Persiste no PostgreSQL        
4. Backend atualiza status    
5. Dashboard consome dados agregados (com Redis)    
6. IA gera insights de forma assíncrona    

---

## Modelo de uso

O usuário poderá:

- Inserir manualmente transações    
- Ou importar via CSV    
- Visualizar dashboard mensal    
- Visualizar previsibilidade financeira    
- Receber insights em momentos estratégicos    

---
