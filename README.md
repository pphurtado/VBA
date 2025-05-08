# Calculadora de Propiedades Termodinámicas: Osciladores Armónicos Unidimensionales

Este proyecto es una **aplicación interactiva en Streamlit** que permite calcular y visualizar propiedades termodinámicas de un sistema clásico compuesto por \( N \) osciladores armónicos unidimensionales. Está orientado a propósitos educativos e ilustrativos dentro del contexto de la **física estadística**.

## 🧪 Fundamento Teórico

El sistema está basado en el Hamiltoniano clásico:

\[
H = \sum_{i=1}^N \left( \frac{p_i^2}{2m} + \frac{1}{2} m (2\pi \nu)^2 x_i^2 \right)
\]

La región accesible del espacio fásico está delimitada por \( H \leq E \), lo que define una hiperesfera en \( 2N \) dimensiones. El volumen acumulado \( \Gamma_N(E) \) y la densidad de estados \( \Omega_N(E) \) se calculan de dos formas posibles, dependiendo de la elección del usuario:

- **Con unidades completas**: incluye masa, frecuencia angular y constante de Planck.
- **Adimensional**: usa la forma \( (E / h\nu)^N \), más simplificada.

## ⚙️ Funcionalidad

La app permite al usuario:

- Elegir el número de osciladores \( N \)
- Ingresar energía total \( E \), masa \( m \), frecuencia \( \nu \) y constante de Planck \( h \)
- Escoger el modo de cálculo del volumen fásico
- Obtener:
  - Volumen fásico \( \Gamma(E) \)
  - Densidad de estados \( \Omega(E) \)
  - Entropía \( S(E) = k_B \ln \Omega(E) \)
- Visualizar gráficos interactivos de:
  - \( \Gamma(E) \) y \( \Omega(E) \) frente a la energía
  - Representación del contorno energético en el espacio fásico (solo para \( N = 1 \))

## 📊 Tecnologías utilizadas

- **Python 3**
- **[Streamlit](https://streamlit.io/)** para la interfaz web
- **NumPy** y **SciPy** para cálculos numéricos y funciones especiales
- **Matplotlib** para la visualización gráfica

## ▶️ Cómo ejecutar

1. Asegúrate de tener Python instalado.
2. Instala las dependencias necesarias:
   ```bash
   pip install streamlit numpy scipy matplotlib
