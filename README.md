# Pizzería - Gestión en Kotlin

Aplicación de consola para gestionar clientes, productos (pizzas, combos, bebidas, ingredientes) y pedidos, aplicando conceptos avanzados de Kotlin.

## Cómo ejecutar

1. Abrir el proyecto en IntelliJ IDEA (JDK 17 o superior).
2. Sincronizar Gradle.
3. Ejecutar `main()` en `Main.kt`.
4. Probar rápido: opción `9` (datos de ejemplo) y luego `8` (resumen).

## Estructura y requisitos

| Paso | Requisito | Archivo |
|---|---|---|
| 1 | Validación de correo y teléfono (Regex) | `Validaciones.kt` |
| 1 | Rango de fechas (promoción) y rango de cantidad 1-100 | `Validaciones.kt` |
| 2 | Anotación `@Promocionable` | `Promocionable.kt`, `Producto.kt` |
| 2 | Reflection (propiedades y métodos) | `Reflexion.kt` |
| 3 | Operador `+` en `Pedido` | `Pedido.kt` |
| 3 | Operador `==` en `Producto` (equals) | `Producto.kt` |
| 4 | Desestructuración de `Cliente` y `Pedido` | `Cliente.kt`, `Pedido.kt`, `Main.kt` |
| 5 | `equals()` y `hashCode()` en `Cliente` y `Producto`, sin duplicados | `Cliente.kt`, `Producto.kt`, `Main.kt` |
| 6 | Resumen integrador | `Resumen.kt` (opción 8 del menú) |

## Menú

1. Registrar cliente
2. Crear pedido
3. Ver pedidos
4. Ver promocionables
5. Analizar clase (reflection)
6. Combinar dos pedidos
7. Registrar producto
8. Ver resumen
9. Cargar datos de ejemplo
0. Salir

## Notas

- El período de promoción es noviembre de 2026. Para ver el descuento, ingresar una fecha dentro de ese mes al crear un pedido.
- Teléfonos: 12 dígitos con formato `+XX (XXX) XXX-XXXX`.
