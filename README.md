# Análise de dados da NBA com SQL

Projeto acadêmico desenvolvido em equipe no módulo 3 da Resilia, com exploração de estatísticas da NBA por meio de SQL e apresentação dos resultados. Este repositório preserva os arquivos do trabalho original e organiza sua leitura como parte do portfólio de Rafael Peruzini.

## Material disponível

| Arquivo ou pasta | Conteúdo |
| --- | --- |
| [nba.sql](nba.sql) | Consultas exploratórias originais sobre jogadores, minutos, assistências e equipes |
| [NBA.pptx](NBA.pptx) | Apresentação produzida para o projeto |
| `queries/` e `tables/` | Pastas do projeto original; atualmente contêm apenas arquivos marcadores |
| `Link do trello` | Referência ao quadro utilizado na organização do trabalho |

O repositório contém as consultas e a apresentação, mas não contém os CSVs nem o script de criação das tabelas. Não há arquivo Power BI publicado nesta cópia do projeto.

## Perguntas exploradas

- Como comparar o tempo em quadra dos jogadores?
- Quais jogadores se destacam em assistências?
- Como relacionar estatísticas de equipes e seus cadastros?
- Como organizar consultas SQL e comunicar uma análise em equipe?

## Tecnologias

SQL com sintaxe de MySQL, MySQL Workbench e Git/GitHub. As consultas referenciam as tabelas `games_details`, `players`, `rankings`, `teams` e `games`.

## Examinar o projeto

```bash
git clone https://github.com/Peruzini/M3-NBA-DataAnalytics-SQL.git
cd M3-NBA-DataAnalytics-SQL
```

Comece pela apresentação e pelo arquivo `nba.sql`. Para executar as consultas, é necessário obter a base usada no trabalho, conferir sua origem e permissão de uso, criar as tabelas e importar os dados em uma instância de MySQL. O Workbench é o cliente de acesso; ele depende de um servidor de banco de dados disponível.

A documentação original apontava ao [repositório de Mauro Mendes](https://github.com/maurocmendes/M3-NBA-DataAnalytics-SQL). Esse link é mantido como referência histórica da equipe, sem pressupor que todos os dados continuem disponíveis nele.

## Cuidados na interpretação das consultas originais

As consultas foram preservadas como material acadêmico. Antes de reutilizá-las em uma análise atual, revise:

- O tipo de `MIN`: uma duração em texto precisa ser convertida antes de comparar ou calcular médias.
- A granularidade e as chaves de agrupamento: selecionar jogador e agrupar apenas por assistências pode produzir resultados inválidos ou ambíguos.
- A tabela de classificação: contar registros de `W` não equivale a somar vitórias, e fotografias acumuladas de classificação não devem ser somadas indiscriminadamente.
- As junções por jogador: se o cadastro tiver várias temporadas por jogador, uma junção somente por ID pode multiplicar linhas.

Não foram publicados novos resultados numéricos nesta revisão, pois a base original não está incluída no repositório. Os [estudos demonstrativos de BI](https://github.com/Peruzini/NOVOREPOSIT) apresentam exemplos reproduzíveis com dados sintéticos e validações.

## Equipe do projeto original

- [Yasmin Ramos](https://github.com/yasminramos)
- [Breno Garduci](https://github.com/Garduciz)
- [Rafael Peruzini](https://github.com/Peruzini)
- [Tulio Roberto](https://github.com/tuliorsc10)
- [Mauro Mendes](https://github.com/maurocmendes)

Os créditos do trabalho em equipe foram preservados. Esta página não atribui a execução integral do projeto a um único participante.

## Referências

- [NBA Stats](https://www.nba.com/stats/)
- [Documentação do MySQL](https://dev.mysql.com/doc/)

O README original mencionava MIT, mas esta cópia não inclui um arquivo de licença. Confirme os termos aplicáveis antes de redistribuir materiais de terceiros.
