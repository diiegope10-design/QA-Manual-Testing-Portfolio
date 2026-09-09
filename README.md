# QA Manual Testing Portfolio

Portfolio de proyectos de testing manual, orientado a demostrar el dominio de técnicas de diseño de casos de prueba, ejecución, reporte de bugs y ciclos de re-testing/regresión sobre aplicaciones web reales.

---

## 📁 Proyecto 1 – Testing Funcional en SauceDemo

**Aplicación bajo prueba:** [SauceDemo](https://www.saucedemo.com)
**Tipo de testing:** Funcional – Caja negra
**Entorno:** Google Chrome / Windows / Desktop
**Casos ejecutados:** 10 (10 PASS)

### Objetivo
Validar el flujo completo de un e-commerce: login, visualización de productos, carrito de compras y checkout, cubriendo tanto escenarios positivos como negativos.

### Alcance
- Inicio de sesión con credenciales válidas e inválidas (usuario vacío, contraseña vacía, ambos vacíos, credenciales incorrectas)
- Visualización del listado de productos tras autenticarse
- Agregado de producto al carrito
- Checkout con datos incompletos (validación de campos obligatorios)
- Checkout completo con confirmación de compra

### Resultado
10/10 casos ejecutados con resultado exitoso. El sistema respondió de forma consistente con los mensajes de error esperados (`Epic sadface: ...`) en todos los escenarios negativos.

📄 [Ver casos de prueba completos](./📄%20Proyecto%201%20%E2%80%93%20Testing%20QA%20Manual%20_%20SauceDemo%20-%20Hoja%201.pdf)

---

## 📁 Proyecto 2 – Técnicas de Diseño y Ciclo de Pruebas en ParaBank

**Aplicaciones bajo prueba:** [ParaBank](https://parabank.parasoft.com) / [QA Journey – Form Validation](https://playground.qajourney.net/form/)
**Tipo de testing:** Funcional — Técnicas de caja negra (Partición de Equivalencias, Valor📄 [Ver casos de prueba completos](./Proyecto-1-SauceDemo-Test-Cases.pdf)es Límite) + Smoke Testing, Bug Reporting, Re-testing y Regression Testing

### Objetivo
Aplicar un ciclo de QA completo — desde el diseño de casos con técnicas formales hasta la detección, documentación y seguimiento de defectos — sobre una aplicación bancaria real.

### Técnicas aplicadas

| Técnica | Aplicación | Casos | PASS | FAIL | Resultado |
|---|---|---|---|---|---|
| Smoke Testing | ParaBank | 5 | 5 | 0 | ✅ OK |
| Validación de Formularios | ParaBank | 3 | 3 | 0 | ✅ OK |
| Partición de Equivalencias | QA Journey | 3 | 3 | 0 | ✅ OK |
| Valores Límite | QA Journey | 4 | 3 | 1 | ⚠️ 1 defecto detectado |
| Bug Reporting | ParaBank | 3 | — | — | 🐞 3 defectos reportados (BUG-001, BUG-002, BUG-003) |
| Re-testing | ParaBank | 2 | 0 | 2 | ❌ Defectos persisten (BUG-001, BUG-002) |
| Regression Testing | ParaBank | 3 | 2 | 1 | ⚠️ Defecto detectado (BUG-003) |
| **TOTAL** | — | **23** | **16** | **4** | **3 defectos reproducibles** |

### Conclusión
Se aplicó un ciclo completo de QA manual: diseño de casos con técnicas formales de caja negra (Partición de Equivalencias, Valores Límite) sobre QA Journey, Smoke Testing y documentación de defectos sobre ParaBank, con seguimiento posterior vía Re-testing y Regression Testing. Se identificaron y reportaron 3 defectos reproducibles en la funcionalidad de transferencias de ParaBank, dos de los cuales persistieron tras el re-testing.

📄 [Ver casos de prueba completos](./Proyecto%202%20%E2%80%94%20T%C3%A9cnicas%20de%20dise%C3%B1o%20%2B%20ciclo%20de%20pruebasculo%20sin%20t%C3%ADtulo%20-%20Hoja%201.pdf)
