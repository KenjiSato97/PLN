1. Objetivo
O objetivo deste trabalho é analisar os discursos proferidos no Conselho de Segurança da ONU para identificar padrões e tendências sem a necessidade de rótulos prévios, utilizando técnicas de classificação não supervisionada. Através dessa abordagem, buscamos entender melhor os tópicos predominantes nas discussões e as relações entre diferentes países e seus posicionamentos.

2. Apresentação
2.1 Base de Dados
Este projeto utiliza um conjunto de dados contendo os debates do Conselho de Segurança da ONU entre janeiro de 1995 e dezembro de 2020. Os dados foram extraídos de protocolos oficiais das reuniões, divididos em discursos distintos. Para cada discurso, são fornecidos metadados como:

O orador (nome e país)
O papel do orador na reunião
O tema abordado
O corpus contém 82.165 discursos extraídos de 5.748 atas de reuniões, conforme os dados de Schoenfeld et al. 2019.

2.2 DistilBERT
O modelo DistilBERT é uma versão mais compacta e eficiente do BERT, com a mesma arquitetura geral, mas com algumas modificações. Ele possui:

A remoção dos embeddings do tipo token e do pooler.
A redução do número de camadas pela metade.
Melhor otimização das operações do Transformer para maior eficiência computacional.
Comparado ao BERT, o DistilBERT é 40% menor, 60% mais rápido e retém 97% da capacidade de compreensão de linguagem, conforme descrito em Sanh et al. 2019.

2.3 K-Means
O K-Means é um algoritmo de agrupamento utilizado para identificar padrões em conjuntos de dados. Ele funciona mapeando cada observação no conjunto de dados para um ponto em um espaço de n dimensões, onde n é o número de atributos da observação. O algoritmo busca agrupar as observações em clusters (ou grupos) com base na similaridade entre elas.

Exemplo: Para um conjunto de dados com atributos como temperatura e umidade, o K-Means agrupa as observações em clusters de pontos no espaço bidimensional.
Esse método foi utilizado para agrupar os discursos em tópicos similares com base nas palavras e contextos mais frequentes, ajudando a identificar tendências e padrões nos debates.

2.4 Word Cloud (Nuvem de Palavras)
A Word Cloud (ou nuvem de palavras) é uma representação visual das palavras mais frequentes em um conjunto de dados de texto. O tamanho de cada palavra na nuvem é proporcional à sua frequência ou importância, permitindo visualizar rapidamente quais palavras são mais proeminentes em um determinado conjunto de dados.

A ferramenta de nuvem de palavras foi utilizada neste projeto para visualizar as palavras mais recorrentes nos discursos analisados, facilitando a interpretação dos tópicos predominantes nas discussões do Conselho de Segurança da ONU.
