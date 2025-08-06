# 📊 Python para Cientistas — Regressão Linear Clássica vs. Machine Learning (IA)

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-1.21%2B-orange)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-brightgreen)](https://matplotlib.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-red)](https://scikit-learn.org/)

Este repositório contém um **notebook Jupyter** que aplica **Machine Learning (Regressão Linear)** para prever o **potencial de parada** em um experimento de determinação da **constante de Planck** usando uma **célula fotoelétrica**.

---

## 🔍 Diferença para o notebook anterior
📄 **Notebook anterior**: utilizava **estatística clássica (mínimos quadrados)** com base na **equação física conhecida**:

\[
eV_p = h\nu - W
\]

- Você **define o modelo** previamente (a fórmula física).
- O ajuste serve para encontrar os parâmetros \( h \) e \( W \).
- Não há "aprendizado" no sentido de IA — apenas cálculo determinístico.

🤖 **Este notebook**: aplica **Machine Learning supervisionado** (`LinearRegression` do scikit-learn) para **aprender diretamente dos dados** a relação entre a frequência \( \nu \) e o potencial de parada \( V_p \), **sem precisar informar explicitamente a equação física**.

- O algoritmo **aprende** o padrão matemático.
- Pode **prever valores** para frequências que não estavam nos dados originais.
- É considerado IA porque generaliza padrões para novos dados.

---

## 📦 Pacotes Utilizados
- Python 3.8+
- NumPy
- Matplotlib
- scikit-learn

---

## 🚀 Executando Localmente
```bash
pip install -r requirements.txt
jupyter notebook Aula_Doutorado_IA_comentado.ipynb
