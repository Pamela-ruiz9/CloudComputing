# Suma de Arreglos en Paralelo con OpenMP (C++)

**Autor:** Ingrid Pamela Ruiz Puga  
**Descripción:** Proyecto en C++ que realiza la suma elemento a elemento de dos arreglos (vectores) utilizando **OpenMP** para paralelizar el ciclo `for` y aprovechar múltiples hilos del procesador.

---

## Objetivo
Implementar una versión paralela de la suma de dos arreglos:

- Dados dos arreglos `A` y `B` con `N` elementos,
- Se genera un tercer arreglo `C` donde:  
  **C[i] = A[i] + B[i]**

La paralelización es posible porque cada suma es **independiente** de las demás.

---

## Tecnologías y herramientas
- **Lenguaje:** C++
- **Entorno:** Visual Studio (Windows)
- **Paralelización:** OpenMP (`#pragma omp parallel for`)

---

## Estructura del proyecto
- `main.cpp`  
  - Genera arreglos `A` y `B` con valores aleatorios  
  - Suma paralelamente para producir `C`  
  - Imprime los primeros elementos para verificación  
  - Mide el tiempo de ejecución con `omp_get_wtime()`  
  - Verifica que el resultado sea correcto

---

## Requisitos
- Visual Studio (recomendado 2019 o 2022)
- Compilador MSVC con soporte OpenMP

---

## Configuración en Visual Studio (OpenMP)
1. Clic derecho al proyecto → **Properties**
2. **Configuration Properties → C/C++ → Language**
3. Activar: **OpenMP Support** → `Yes (/openmp)`
4. Apply → OK

---

## Cómo ejecutar
1. Abrir el proyecto en Visual Studio
2. Compilar y ejecutar: **Ctrl + F5**
3. El programa mostrará:
   - Los primeros elementos de `A`, `B` y `C`
   - Tiempo de ejecución
   - Resultado de verificación (CORRECTO / ERROR)

---

## Ejemplo de salida esperada

<img width="1920" height="1037" alt="Pame_tarea" src="https://github.com/user-attachments/assets/3bbef882-6d22-4583-bbad-8151099d397d" />

