# Sistema de Inventario y Ventas

Sistema administrativo para gestionar productos, proveedores, clientes y ventas con control de stock automático.

Monorepo compuesto por dos repositorios independientes enlazados como submódulos de Git.

## Repositorios

| Carpeta | Repositorio | Descripción |
|---|---|---|
| `sistema-inventario-ws/` | [sistema-inventario-ws](https://github.com/RamonCheno/sistema-inventario-ws) | Servicio WCF SOAP en C# |
| `sistema-inventario-ui/` | [sistema-inventario-ui](https://github.com/RamonCheno/sistema-inventario-ui) | Aplicación React + TypeScript |

## Stack

**Backend**
- C# / .NET Framework 4.8
- WCF SOAP (.svc)
- Entity Framework 6
- SQL Server LocalDB

**Frontend**
- React 19 + TypeScript
- Vite + pnpm
- React Router
- React Hook Form + Zod

## Clonar el proyecto completo

```bash
git clone --recurse-submodules https://github.com/RamonCheno/sistema-inventario.git
```

Si ya clonaste sin `--recurse-submodules`:

```bash
git submodule update --init --recursive
```

## Estructura

```
sistema-inventario/
├── sistema-inventario-ws/         ← submódulo: sistema-inventario-ws
│   ├── wcf-clasico/               ← WCF SOAP clásico (.NET Framework 4.8) — en uso
│   └── corewcf-net10/             ← CoreWCF sobre .NET 10 (aprendizaje, en progreso)
└── sistema-inventario-ui/         ← submódulo: sistema-inventario-ui (React)
```

## Contexto

Proyecto desarrollado como parte del roadmap de aprendizaje React JS → React Native.
Fase 2 — React JS Avanzado + WCF SOAP.
