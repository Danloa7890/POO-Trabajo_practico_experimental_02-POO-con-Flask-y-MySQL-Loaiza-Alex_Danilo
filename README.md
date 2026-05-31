# Caso de Estudio POO — Sistema de Reservas de Laboratorio

Este proyecto implementa un sistema de gestión de reservas de laboratorios universitarias utilizando una arquitectura en capas con principios SOLID en Python y una base de datos MySQL sin ORM.


## Estructura del Proyecto

```text
proyecto/
├── app/
│   ├── __init__.py                         ← Bootstrap: inicializa Flask y dependencias
│   ├── api/
│   │   ├── __init__.py                     ← (vacío)
│   │   └── reserva_controller.py           ← Capa de interfaz REST (HTTP)
│   ├── domain/
│   │   ├── __init__.py                     ← (vacío)
│   │   ├── entities.py                     ← Entidades y objetos de valor
│   │   ├── exceptions.py                   ← Excepciones de dominio
│   │   └── repository.py                   ← Interfaz abstracta del repositorio
│   ├── infrastructure/
│   │   ├── __init__.py                     ← (vacío)
│   │   ├── db_pool.py                      ← Pool de conexiones MySQL
│   │   ├── reserva_dao.py                  ← Acceso a datos (SQL puro)
│   │   └── mysql_reserva_repository.py     ← Implementación del repositorio
│   └── application/
│       ├── __init__.py                     ← (vacío)
│       └── reserva_service.py              ← Casos de uso / lógica de aplicación
├── .env                                    ← Variables de entorno (no subir)
├── .gitignore
├── requirements.txt
├── schema.sql                              ← DDL de la base de datos
└── run.py                                  ← Punto de entrada de la aplicación
```
