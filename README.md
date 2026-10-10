# Cesta em Perspectiva

Site estático para acompanhar o custo da cesta básica durante os governos Bolsonaro (2019–2022) e Lula (2023 em diante), com valores nominais e corrigidos pelo IPCA geral.

## Dados e metodologia

- Custos mensais: relatórios públicos da Pesquisa Nacional da Cesta Básica de Alimentos do [DIEESE](https://www.dieese.org.br/analisecestabasica/analiseCestaBasicaAnteriores.html).
- Correção: número-índice mensal do IPCA geral do Brasil, [IBGE/SIDRA, tabela 1737](https://sidra.ibge.gov.br/tabela/1737).
- Referência monetária: agosto de 2026.
- Cobertura: 17 capitais; dezembro de 2018 a agosto de 2026, incluindo a base anterior ao primeiro mandato comparado.
- Fórmula: preço nominal × índice do mês de referência ÷ índice do mês observado.

A composição da cesta varia por região. Há dois valores não publicados: Brasília em novembro de 2019 e Belo Horizonte em maio de 2021. Revisões com valores explícitos foram incorporadas e possuem links para suas fontes. Belo Horizonte tem uma ressalva sobre recálculo histórico ainda não integralmente incorporado. A metodologia e as limitações aparecem no site.

Os dados são uma fotografia coletada em 10/10/2026, sem atualização automática. Uma variação durante um governo não demonstra causalidade.

## Rodar localmente

Com Python instalado, na pasta do repositório:

```sh
python -m http.server 8765 --directory docs
```

Acesse http://localhost:8765.

## Publicação

GitHub Pages publica a pasta `docs` da branch `main`. As atualizações desses arquivos são publicadas automaticamente pelo GitHub. Não há dependências de compilação ou login para visitantes.

Os dados e a metodologia pertencem às respectivas fontes; este projeto não é afiliado ao DIEESE ou ao IBGE.
