# Among Us: Sem Limites (Reactor)

Projeto inicial para gerar uma DLL de mod usando o template oficial do Reactor e GitHub Actions.

## O que este pacote faz agora
- Prepara um workflow do GitHub Actions para instalar o template oficial `Reactor.Template`.
- Compila o projeto de exemplo e publica as DLLs como artefato para download.
- Documenta o alvo pretendido: cooldowns e tarefas configuráveis de 0 a 9999.

## Limitação importante
Este é um **bootstrap de compilação**, não uma implementação pronta das regras do jogo. O código que altera os cooldowns e as tarefas precisa ser adaptado às classes e aos métodos presentes na build exata de Among Us de 2026. A API Reactor ajuda a desenvolver mods, mas não fornece automaticamente uma API universal para mudar todas as opções do jogo. Não seria correto afirmar que uma DLL já altera essas regras ou que só o anfitrião basta sem testar a sincronização multiplayer.

## Como gerar a DLL
1. Crie um repositório vazio no GitHub.
2. Extraia todos os arquivos deste ZIP e envie-os para a raiz do repositório.
3. Abra a aba **Actions**.
4. Se necessário, habilite GitHub Actions para o repositório.
5. Execute **Build Reactor starter** em **Run workflow** (ou faça um push).
6. Quando terminar com sucesso, abra a execução e baixe o artefato `among-us-sem-limites-starter`.

O artefato contém a DLL gerada pelo template oficial. É um ponto inicial de modding, não a versão funcional “Sem Limites”.

## Instalação do ambiente
Para carregar mods Reactor, siga a documentação oficial do Reactor e instale BepInEx e Reactor compatíveis com a versão do jogo:
- https://docs.reactor.gg/
- https://github.com/NuclearPowered/Reactor
- https://github.com/NuclearPowered/Reactor.Template

Não instale DLLs aleatórias em partidas públicas. Teste primeiro em Freeplay ou sala privada.
