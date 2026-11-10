# Trégua

Comunicação segura entre pais separados em conflito.

Trégua é um projeto de código aberto e interesse público. A proposta é um canal de comunicação com inteligência artificial e supervisão humana para que pais separados em alto conflito tratem de filhos, pensão e visitas sem contato hostil, com registro organizado que pode ser apresentado como prova.

**Estágio:** protótipo demonstrativo. Ainda não testado com usuárias.

## O problema

Quando um casal com filhos se separa, a relação acaba, mas as obrigações continuam por anos. Quando há histórico de violência, a conversa obrigatória sobre os filhos vira o canal pelo qual ela continua, e quem sofre precisa reunir provas por conta própria.

Em 2024 o Brasil registrou 428.301 divórcios. Entre os judiciais, 45,8% eram de famílias só com filhos menores, e a guarda compartilhada (44,6%) superou pela primeira vez a guarda materna. Fonte: IBGE, Estatísticas do Registro Civil 2024.

## O que o protótipo demonstra

- **Linguagem:** a mensagem é analisada antes da entrega. Se houver ofensa, ameaça, pressão financeira ou manipulação, quem escreveu recebe uma versão objetiva e escolhe entre enviá-la ou reescrever. O texto original é preservado no registro.
- **Obrigações:** pensão, convivência e despesas do acordo em lista e calendário, com situação de cada item. A leitura de um acordo é simulada e passa por conferência humana.
- **Registro:** linha do tempo com data e hora e relatório em texto.
- **Supervisão:** mensagens com sinal de ameaça entram na fila de uma profissional, que confirma ou corrige a avaliação e registra uma orientação.

## O que é simulado

- A análise das mensagens é feita por listas de palavras e expressões, na função `analisar` do arquivo `index.html`. Não há modelo de linguagem.
- Todas as pessoas e dados são fictícios e ficam apenas na memória do navegador. Ao recarregar a página, a demonstração volta ao início.
- Não há cadastro, banco de dados nem envio de informações.

## Como ver

Abra o arquivo `index.html` em um navegador. Não é preciso instalar nada.

## Próximos passos

1. Substituir a análise simulada por um modelo de linguagem, com avaliação de erros e de vieses.
2. Testar com usuárias e com profissionais do sistema de justiça.
3. Definir proteção de dados e consentimento conforme a LGPD.
4. Incluir botão de saída rápida e demais cuidados de segurança para quem está em situação de violência.
5. Separar o código em uma aplicação com estrutura própria para receber contribuições.

## Quando não usar

Se houver medida protetiva com proibição de contato, a ferramenta só deve ser usada com autorização judicial.

## Como contribuir

Sugestões e correções são bem-vindas pela aba Issues deste repositório. Pessoas das áreas de engenharia de IA, dados, design, psicologia, serviço social e direito são especialmente bem-vindas.

## Princípios

- O código é aberto. Os dados das famílias, nunca.
- A IA faz a triagem. A decisão é sempre de uma pessoa.
- O texto original nunca é apagado.

## Licença

GNU Affero General Public License v3.0. Veja o arquivo LICENSE.

## Autoria

Projeto idealizado por Paloma Daniele da Silva Freitas, advogada. Protótipo desenvolvido com apoio de ferramentas de IA.

---

Em perigo imediato, ligue 190. Central de Atendimento à Mulher: 180.
