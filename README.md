# Uma Abordagem Espectral-Geométrica para a Conjectura Forte de Goldbach

[![Status](https://img.shields.io/badge/Status-Preprint-blue.svg)]()
[![LaTeX](https://img.shields.io/badge/LaTeX-Source_Code-success.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://img.shields.io/badge/10.5281/zenodo.20678499-blue.svg)](https://doi.org/10.5281/zenodo.20678499)

Este repositório contém o código-fonte LaTeX e o manuscrito do artigo **"Uma Abordagem Espectral-Geométrica para a Conjectura Forte de Goldbach: Uma Prova Condicional via Variedades de Arakelov"**. 

O artigo propõe uma nova estrutura teórica para o tratamento analítico da Conjectura Forte de Goldbach, unificando a Teoria Analítica dos Números clássica com a Geometria Espectral.

## 📄 Resumo do Artigo

A pesquisa estabelece um **Teorema de Equivalência**: demonstra-se rigorosamente que, sob a égide da **Hipótese de Riemann (HR)**, a Conjectura Forte de Goldbach é verdadeira para todo inteiro par suficientemente grande. 

O diferencial metodológico desta abordagem é a **geometrização da distribuição dos números primos**. Em vez de tratar a soma aditiva puramente através da combinatória de crivos, o problema é mapeado como um fluxo de geodésicas em uma variedade Riemanniana de 5 dimensões ($\mathcal{M} = \mathbb{H}^3 \times \mathbb{T}^2$).

### Pilares da Demonstração
1. **O Espaço de Fase:** A variedade $\mathbb{H}^3 \times \mathbb{T}^2$ modela a divergência ergódica das trajetórias primas e impõe o confinamento topológico (sincronização de fase) necessário para a intersecção focal $p_1 + p_2 = 2n$.
2. **Método do Círculo:** Utilização das Somas de Weyl ponderadas integradas sobre o toro $\mathbb{T}^2$.
3. **Controle Espectral do Erro:** Aplicação da Fórmula Explícita de Weil para mapear os zeros da função Zeta de Riemann, garantindo que o termo de erro nos arcos menores seja estritamente limitado a $\mathcal{O}(n^{1/2} \ln^2 n)$.
4. **Positividade da Série Singular:** Prova formal de que a densidade de estados $\mathfrak{S}(2n)$ é estritamente positiva ($\geq 1.32$), impedindo o colapso do termo principal.

## ⚠️ Natureza Condicional da Prova

A honestidade e o rigor matemático são premissas deste trabalho. Declara-se explicitamente que **esta é uma prova condicional**. A validade da limitação do termo de erro e, consequentemente, a positividade estrita da função de contagem de Goldbach $R(2n)$ dependem do limite analítico fornecido pela Hipótese de Riemann (onde a parte real dos zeros não-triviais é exatamente $1/2$).

## 🛠️ Como Compilar o Manuscrito

O arquivo principal é escrito em LaTeX padrão, sem dependências de pacotes não convencionais.

### Via Overleaf (Recomendado)
1. Baixe o arquivo `main.tex`.
2. Crie um novo projeto "Blank Project" no [Overleaf](https://www.overleaf.com/).
3. Substitua o conteúdo do `main.tex` do Overleaf pelo conteúdo baixado.
4. Clique em **Recompile** (Certifique-se de que o compilador está configurado como `pdfLaTeX`).

### Compilação Local
Se você possui o TeX Live ou MiKTeX instalado localmente, rode o seguinte comando no terminal:
```bash
pdflatex main.tex
pdflatex main.tex # Rodar duas vezes para gerar o sumário e referências corretamente
