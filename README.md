# Algoritmos de Otimização - Transporte de Produtos

Este repositório contém a implementação de um problema de otimização de transporte de produtos utilizando três diferentes algoritmos de otimização: **Hill Climbing**, **Simulated Annealing** e **Algoritmo Genético**. O problema foi proposto no curso [Inteligência Artificial e Machine Learning: O Guia Completo](https://www.udemy.com/course/inteligencia-artificial-machine-learning-guia-completo/?couponCode=MTST7102224A2).

## Descrição do Problema

A questão consiste em selecionar produtos para transporte respeitando um limite de espaço disponível. Cada produto tem um valor e ocupa um espaço específico. O objetivo é encontrar a combinação de produtos que maximize o valor transportado sem exceder o espaço disponível.

### Produtos disponíveis:

- Cada produto possui três atributos: **nome**, **espaço que ocupa** e **valor**.

### Restrições:

- O espaço total disponível para transporte é limitado a 3.0 do peso.

O desafio é resolver este problema de forma eficiente utilizando técnicas de otimização.

## Solução

A solução foi implementada no arquivo `transporte.py`, que faz uso da biblioteca `mlrose` para aplicar três diferentes algoritmos de otimização:

1. **Hill Climbing**: Um algoritmo de subida de encosta que ajusta incrementalmente uma solução inicial.

2. **Simulated Annealing**: Algoritmo inspirado no processo de resfriamento de metais, que aceita soluções temporariamente piores para escapar de ótimos locais.

3. **Algoritmo Genético**: Um algoritmo baseado em evolução, que gera uma população de soluções e utiliza operadores genéticos como cruzamento e mutação para encontrar soluções melhores.

### Como Executar

1. **Instalação das Dependências**:

   Você pode instalar a versão mais recente diretamente do GitHub:

   ```bash
   pip install https://github.com/gkhayes/mlrose/archive/refs/heads/master.zip
   ```

2. **Execução do Arquivo Principal**:

   Para resolver o problema e visualizar a solução, execute o arquivo `transporte.py`:

   ```bash
    python transporte.py
   ```

   Esse arquivo contém a implementação da função de avaliação, a representação dos produtos e a execução dos três algoritmos de otimização. Após a execução, os produtos selecionados serão impressos no terminal.
