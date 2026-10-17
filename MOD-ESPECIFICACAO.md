# Especificação funcional — Sem Limites

Configurações pretendidas:
- Cooldowns: 0–9999 segundos.
- Tarefas comuns, longas e curtas: 0–9999.
- Validação de entrada para impedir valores fora do intervalo.
- Aplicação das alterações apenas quando o jogador local é o anfitrião.
- Teste de sincronização em sala privada com clientes sem o mod.

## Próxima etapa de implementação
A implementação precisa referenciar as classes geradas para a versão instalada do Among Us e confirmar como as opções de lobby são serializadas/sincronizadas nessa versão. Só depois disso dá para escrever os patches específicos para cooldowns e tarefas sem inventar nomes de métodos ou produzir uma DLL que falhe ao carregar.
