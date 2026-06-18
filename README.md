# Projeto final - Visualizador 3D de Moléculas
**Autora:** Maria Vitória Dias Meneses
<br>
**Instituição:** Ilum Escola de Ciência / CNPEM
<br>
**Disciplina:** Práticas Básicas em Ciência de Dados
 
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
 
Para executar o notebook, instale as bibliotecas necessárias rodando a célula de instalação no início do próprio notebook, ou manualmente:
 
```bash
pip install rdkit plotly networkx pubchempy ipywidgets
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
 
*Desenvolvido com Python 3.13 em JupyterLab.*
