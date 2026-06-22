![Imagem Ilum](header_ilum.png)

# Projeto final - Visualizador 3D de Moléculas
**Autora:** Maria Vitória Dias Meneses (https://github.com/mavidiias)
<br>
**Instituição:** Ilum Escola de Ciência / CNPEM
<br>
**Disciplina:** Práticas Básicas em Ciência de Dados
<br>
**Professores Responsáveis:**
<ul>
  <li>Prof. Dr. Daniel Roberto Cassar (https://github.com/drcassar)</li>
  <li>Prof. Dr. James Moraes de Almeida (https://github.com/jamesmalmeida)</li>
  <li>Prof. Dr. Leandro Nascimento Lemos (https://github.com/llemos)</li>
</ul>
 
---
 
## Sobre o projeto
 
Este projeto une dois conceitos centrais da disciplina — **grafos** e **ciência de dados** — aplicados à visualização de estruturas moleculares em três dimensões.
 
A ideia central é simples: uma molécula é, matematicamente, um grafo. Cada átomo é um nó e cada ligação química é uma aresta. A partir dessa representação, é possível não só visualizar a geometria da molécula no espaço, mas também extrair propriedades estruturais diretamente da teoria dos grafos, como grau dos nós, diâmetro e conectividade.
 
O usuário fornece uma notação SMILES — padrão amplamente utilizado em química computacional — e o programa gera automaticamente a estrutura 3D interativa da molécula, junto com uma análise do grafo correspondente.
 
---
 
## Como navegar pelo repositório
 
O projeto está inteiramente contido em um único notebook Jupyter. **Para ver o projeto completo, abra o arquivo `visuamolecula.ipynb`.**
 
O notebook está organizado com começo, meio e fim, guiando o leitor por cada etapa do processo: da motivação do projeto, passando pela implementação comentada, até os resultados e discussão. Basta executar as células em ordem.
 
```
📁 repositório
│
├── .gitignore
├── LICENSE
├── visuamolecula.ipynb   ← abra este arquivo para ver o projeto completo
└── README.md
```
 
---
 
## Pré-requisitos
 
Para executar o notebook, instale as bibliotecas necessárias rodando a célula abaixo no próprio notebook:
 
```bash
!pip install rdkit plotly networkx pubchempy ipywidgets
```
 
Após a instalação, reinicie o kernel do JupyterLab antes de executar o restante do notebook.
 
---
 
## Funcionalidades
 
- Geração de coordenadas 3D a partir de notação SMILES via **RDKit**
- Conversão da molécula em grafo com **NetworkX**
- Análise do grafo: número de átomos, ligações, grau de cada átomo e diâmetro
- Visualização 3D interativa (rotação, zoom) com **Plotly**
- Identificação automática do nome da molécula via **PubChemPy**
---
 
## Tecnologias utilizadas
 
| Biblioteca | Finalidade |
|---|---|
| RDKit | Interpretação do SMILES e geração de geometria 3D |
| NetworkX | Representação e análise da molécula como grafo |
| Plotly | Visualização 3D interativa |
| PubChemPy | Identificação do nome da molécula |
| NumPy | Operações auxiliares |
 
---
 
## Exemplos de moléculas
 
| Molécula | SMILES |
|---|---|
| Água | `O` |
| Metano | `C` |
| Benzeno | `c1ccccc1` |
| Etanol | `CCO` |
| Glicose | `C(C1C(C(C(C(O1)O)O)O)O)O` |
| Cafeína | `Cn1cnc2c1c(=O)n(c(=O)n2C)C` |
 
---

## Referências
 
WEININGER, D. SMILES, a chemical language and information system. 1. Introduction to methodology and encoding rules. **Journal of Chemical Information and Computer Sciences**, v. 28, n. 1, p. 31–36, 1988. DOI: 10.1021/ci00057a005.

<br>

LANDRUM, G. et al. **RDKit: Open-Source Cheminformatics**. Versão 2026.03.2. Disponível em: https://www.rdkit.org. Acesso em: 18 jun. 2026.

<br>

HAGBERG, A. A.; SCHULT, D. A.; SWART, P. J. Exploring network structure, dynamics, and function using NetworkX. In: **Proceedings of the 7th Python in Science Conference (SciPy 2008)**, Pasadena, CA, EUA, ago. 2008. p. 11–15.

<br>

PLOTLY TECHNOLOGIES INC. **Collaborative data science**. Montreal, QC: Plotly Technologies Inc., 2015. Disponível em: https://plotly.com. Acesso em: 18 jun. 2026.

<br>

KIM, S. et al. PubChem 2023 update. **Nucleic Acids Research**, v. 51, n. D1, p. D1373–D1380, 2023. DOI: 10.1093/nar/gkac956.
 
---
 
*Desenvolvido com Python 3.13 em JupyterLab.*
