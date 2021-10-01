# Lab06 - Artigo de Dataset Público

## Aluno
* `240106`: `<Lucas Otávio Nascimento de Araújo>`

## Análise do Artigo `<CandiDATA: um dataset para analise das eleições no Brasil>`

| campo | valor |
|------------|----------------------------------------|
| referência | `Felipe F. Vasconcelos, João V. S. Tavares, Murilo U. Ribeiro, Fabio J. Coutinho, João Paulo Clarindo (2021). CandiDATA: um dataset para análise das eleições no Brasil. *Brazilian Symposium on Databases - Dataset Showcase Workshop*, a publicar` |
| link       | `https://drive.google.com/file/d/10hh-MLRk9omaGwdormsXwQa7O7XHXFhT/view` |
| dataset | `https://github.com/felipeVsc/CandiDATA` |
| formato | `Tabelas em formato CSV, separadas em pastas (por ano) e em arquivos (por unidade federativa)` |

## Resumo

Dados sobre as eleições são essenciais para compreender e avaliar o desenvolvimento da Democracia Brasileira. O Tribunal Superior Eleitoral (TSE) disponibiliza dados sobre candidatos dos pleitos realizados entre 1933 e 2020, que, embora já tenham sido utilizados como base para estudos, contêm muitos problemas: apresentam campos inconsistentes, formatos que variam conforme o pleito, falta de informações importantes e padrões antigos ou pouco escaláveis. O artigo propõe-se a criar CandiDATA: um dataset padronizado sobre as eleições brasileiras de 1945 a 2020. Após analisarem trabalhos relacionados e listarem os problemas dos dados do TSE, os autores criaram módulos em Python que padronizaram, transformaram e consolidaram a base de dados.

## Perguntas de pesquisa/análises

O dataset pode ser utilizado para avaliar a participação de grupos e partidos na política brasileira ao longo do tempo (anos dos pleitos) e espaço (unidades federativas e municípios) e analisar correlações entre certas características dos candidatos e o número de votos recebido. O artigo fornece exemplos da visualização do crescimento da participação feminina nas eleições nas últimas décadas e da distribuição de ocupações dos candidatos nas eleições de 2020. Também é possível avaliar separadamente pleitos municipais e estaduais/federais.
Pelo uso do código de município do IBGE adicionado pelos autores, o dataset pode ser integrado a outros bancos de dados, permitindo a correlação com fatores socioeconômicos, ambientais e de estrutura urbana. Isso possibilitaria a identificação de diferentes tendências a depender das características dos municípios. Por exemplo, seria possível identificar se IDH, PIB per capta, urbanização ou cobertura vegetal aparentam influenciar tendências políticas nas eleições.

## Trabalhos relacionados

* Camargo et al (2016): analisa dados de candidatos a vereador por municípios do Rio Grande do Sul no pleito de 2012. As informações foram extraídas dos dados do TSE, convertidas para o formato CSV, e seus atributos foram padronizados. Foram aplicadas técnicas de mineração de dados, que revelaram como fatores mais importantes para a eleição de um candidato: carreira política, idade, grau de escolarização e gênero. Camargo, A., Silva, R., Amaral, E., Heinen, M., and Pereira, F. (2016). Mineração de dados eleitorais: descoberta de padrões de candidatos a vereador na região da campanha do rio grande do sul. *Revista Brasileira de Computação Aplicada*, 8(1):64–73.
* Filho and Pappa (2015): avalia a distribuição demográfica do Twitter. Inferem-se classe social, gênero e idade com base em informações do perfil e mensagens postadas na rede social. Foram utilizados dados do TSE para comparar uma distribuição demográfica real com a obtida pelos autores. Filho, R. M. and Pappa, G. L. (2015). pg. 137-142. In *PROCEEDINGS OF SATELLITE EVENTS OF THE 30TH BRAZILIAN SYMPOSIUM ON DATABASES*, page 1–320.
* CEPESP (2020): facilita o acesso aos datasets do repositório do TSE, corrigindo alguns problemas dos dados originais, mas restringindo-se ao período de 1998 a 2018. O resultado pode ser acessado no site da CepespData ou por meio do uso de R ou Python para acessar APIs. CEPESP, F. (2020). Cepespdata - banco de dados políticos. <https://empregabrasil.mte.gov.br/76/cbo/>. [Online; acesso em ago. 12].