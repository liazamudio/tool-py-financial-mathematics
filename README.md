# Matemáticas Financieras

Notebooks de Python con las fórmulas y ejercicios prácticos de matemáticas financieras (tasas de interés simple, compuesto y real) para personas y profesionales que toman decisiones financieras.

<!-- COMPLETAR: agregar GIF o captura de pantalla mostrando un notebook en ejecución. No se encontró ninguna imagen/demo en el repositorio. -->

## Problema / Motivación

Este curso está dirigido a personas que toman decisiones financieras (propias o de empresa) y necesitan las bases de valuación: precio de acciones, bonos, derivados, o el costo real de un crédito o compra a plazos. El enfoque es práctico: cada tema se resuelve con casos de uso reales, no solo teoría.

Requisitos previos: aritmética básica (operaciones y despejes) y, opcionalmente, Microsoft Excel para contrastar los ejercicios.

## Demo

<!-- COMPLETAR: no hay una versión en vivo (son notebooks locales). Agregar aquí GIF/capturas de los notebooks ejecutándose, o un link a un entorno como Binder/Google Colab si se desea que los usuarios los prueben sin instalar nada. -->

## Stack técnico

- Frontend: No aplica — el proyecto son notebooks de Jupyter, sin interfaz web.
- Backend: Python 3 (funciones puras, sin servidor)
- Librerías: `pandas`, `numpy`, `math` (estándar de Python)
- Base de datos: No aplica
- Infraestructura/Deploy: No se detectó configuración de despliegue ni CI/CD (sin `Dockerfile`, `docker-compose.yml`, `.github/workflows/`, etc.). Los notebooks están pensados para ejecutarse localmente con Jupyter.

<!-- COMPLETAR: no existe requirements.txt ni pyproject.toml en el repo. Confirmar versión mínima de Python soportada y fijar versiones de pandas/numpy si se desea reproducibilidad exacta. -->

## Características principales

- Construcción de la Tasa de Interés Total (TIT) a partir de riesgo crediticio, riesgo de liquidez y prima temporal (`01-construccion-tasa-de-interes.ipynb`)
- Cálculo de tasa de interés real mediante la ecuación de Fisher (tasa nominal vs. inflación)
- Interés simple: cálculo de tasa, tiempo, valor presente y valor futuro, incluyendo tasas variables por periodo y conversión anual/mensual (`02-interes_simple.ipynb`, `03-interes-simple.ipynb`)
- Generación de tablas de evolución del capital mes a mes con `pandas` (interés acumulado, valor del activo)
- Interés compuesto: cálculo de tasa, tiempo, valor futuro y valor presente, con tasas fijas y variables, y distintas periodicidades de reinversión (`04-interes_compuesto.ipynb`)
- Ejercicios interactivos por consola (`input()`) para capturar montos, plazos y tasas y obtener el resultado

## Cómo correrlo localmente

```bash
# 1. Clonar el repositorio
git clone https://github.com/liazamudio/tool-py-financial-mathematics
cd tool-py-financial-mathematics

# 2. Crear y activar un entorno virtual
python -m venv .venv
.venv\Scripts\activate      # Windows
# source .venv/bin/activate # macOS/Linux

# 3. Instalar dependencias
pip install pandas numpy jupyter

# 4. Levantar Jupyter y abrir cualquier notebook
jupyter notebook
```

No se requieren variables de entorno ni credenciales para ejecutar los notebooks.

## Decisiones técnicas relevantes

<!-- COMPLETAR: documentar por qué se usan notebooks en vez de scripts/módulos reutilizables, por qué no hay un requirements.txt fijado, y cualquier trade-off considerado (p. ej. pandas solo para tablas de amortización vs. cálculo puro con math). -->

## Estado del proyecto

Activo — el último commit registrado es del 2025-12-20 ("Update README with course overview and objectives"), y hay notebooks nuevos sin confirmar en git (`01-construccion-tasa-de-interes.ipynb`, `02-interes_simple.ipynb`, `03-interes-simple.ipynb`) con fecha de modificación del 2026-08-12.

<!-- COMPLETAR: confirmar si el curso sigue en desarrollo activo, está en mantenimiento o ya se dio por concluido. -->

## Autor / Rol

Alexandro Iván Zamudio Romero — autor único (según `LICENSE`).

<!-- COMPLETAR: si el proyecto se desarrolló en equipo, especificar aquí el rol concreto desempeñado. -->

## Licencia

MIT — ver [LICENSE](LICENSE).
