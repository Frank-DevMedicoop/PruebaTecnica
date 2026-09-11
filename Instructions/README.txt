1.1 Ejercicio 1 — Lógica de negocio

Implementar una clase CuentaService (C#, .NET) con almacenamiento en memoria (una lista o diccionario, no base de datos) que exponga:

●	Cuenta CrearCuenta(string numeroCuenta, string nombreSocio, decimal saldoInicial) — el saldo inicial no puede ser negativo.
●	Movimiento Depositar(int cuentaId, decimal monto) — el monto debe ser mayor que cero.
●	Movimiento Retirar(int cuentaId, decimal monto) — no puede dejar el saldo en negativo; el monto debe ser mayor que cero.
●	List<Movimiento> ObtenerHistorial(int cuentaId) — devuelve los movimientos ordenados por fecha descendente.

Los casos inválidos (cuenta inexistente, monto inválido, fondos insuficientes) deben señalizarse de forma clara — con excepciones, un tipo Result, o el mecanismo que el candidato prefiera, siempre que sea explícito y no silencioso.

Incluir al menos 3 pruebas unitarias (xUnit o NUnit) para Depositar y Retirar, cubriendo un caso exitoso y un caso de error cada uno.
