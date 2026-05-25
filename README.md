# Lab8 — Simulación Panini FIFA 2026: Presupuesto e Intercambio
### MM3014 Teoría de Probabilidades · Sección 40 · 2026

**Integrantes:**
- Denil José Parada Cabrera — 24761
- Saúl Esteban Catillo Arenas — 24915

---

## Descripción

Continuación del Lab07. Se extiende la simulación Monte Carlo del álbum Panini FIFA 2026 incorporando dos nuevas variables: un **presupuesto económico fijo** (Etapa 3) y un **mecanismo de intercambio de estampas repetidas** (Etapa 4).


---

## Requisitos

```bash
pip install numpy matplotlib jupyter
```

---

## Cómo ejecutar

```bash
jupyter notebook
```

Abrir `Lab08.ipynb` y ejecutar **Kernel → Restart & Run All**.

---

## Estructura del notebook

### Etapa 3 — Presupuesto y costo (N=100, S=7, precio Q 9.50, presupuesto Q 1,000)
- Simulación de compra secuencial hasta agotar el presupuesto o completar el álbum
- P(completar), E[sobres], E[estampas distintas en casos no exitosos]
- Comparación: sobres sueltos vs caja de 104 (Q 975) vs estrategia mixta

### Etapa 4 — Intercambio de repetidas (K = 1, 2, 5, 10)
- **Parte A:** sobres necesarios para completar el álbum con canje, por valor de K
- **Parte B:** P(completar | M sobres) para cada K; umbrales al 50%, 75% y 90%
- Análisis de rendimientos decrecientes y costo efectivo por estampa canjeada

---

## Parámetros clave

| Parámetro | Valor |
|---|---|
| Semilla | 2026 |
| N (estampas) | 100 |
| S (estampas por sobre) | 7 |
| R (simulaciones) | 10,000 |
| Precio sobre | Q 9.50 |
| Presupuesto (Etapa 3) | Q 1,000.00 |
| Precio caja (104 sobres) | Q 975.00 |
| Valores de K (Etapa 4) | 1, 2, 5, 10 |
