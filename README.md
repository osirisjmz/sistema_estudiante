# sistema_estudiante
Este programa es parte de la actividad dos de la universidad

===========================================================
        OMNIX ACADEMIC SYSTEM - FRAMEWORK V1.0
===========================================================

1. PROPOSITO DEL SISTEMA
-------------------------
Omnix Academic System es una solucion integral de escritorio 
desarrollada en Java para la gestion administrativa de 
instituciones educativas. Permite el control de:
- Registro de Estudiantes y Matriculas.
- Gestion de Personal Docente (Profesores).
- Administracion de Materias y Creditos.
- Control de Evaluaciones y Estatus Academico.

2. ARQUITECTURA "OMNIX ENGINE"
-------------------------------
El sistema implementa las siguientes mejores practicas de ingenieria:

- CONFIGURACION DINAMICA: Uso de 'ConfigLoader' para separar 
  las rutas de archivos del codigo fuente.
- PERSISTENCIA JSON: Almacenamiento ligero por objetos, 
  facilitando la lectura y futuras migraciones.
- AUDITORIA DE RENDIMIENTO: Registro de latencia en milisegundos 
  (ms) para cada operacion clave.
- BAJA LOGICA: Los registros no se borran; se inactivan via 
  status ("Baja", "Inactivo", "Anulado").

3. ESTRUCTURA DE ARCHIVOS RELACIONADOS
--------------------------------------
Para el correcto funcionamiento, el sistema requiere:

A. Configuracion:
   - src/sistema/estudiante/Data/config.txt (Rutas base)

B. Bases de Datos (JSON):
   - estudiantes.json  : Registro de alumnos.
   - data.json         : Datos de Profesores.
   - materias.json     : Catalogo de materias.
   - matriculas.json   : Control de inscripciones.
   - evaluaciones.json : Calendario de examenes.

C. Auditoria (Logs):
   - historylog.txt    : Trazabilidad de operaciones exitosas.
   - error.txt         : Registro de fallos y excepciones.

4. REQUISITOS TECNICOS
-----------------------
- JDK 11 o superior.
- Driver JDBC SQL Server (mssql-jdbc) para modo Online.
- Archivo config.txt correctamente direccionado en DATA_PATH.

5. PALETA DE COLORES OMNIX (UI)
-------------------------------
- AZUL OMNIX (Primario)  : Color(0, 120, 215)
- FONDO OSCURO (Header)  : Color(23, 32, 42)
- FONDO FORMS (Body)     : Color(33, 47, 61)
- VERDE EXITO            : Color(46, 204, 113)
- ROJO ALERTA            : Color(192, 57, 43)

===========================================================
Desarrollado por: Osiris Jimenez (Ocyriz) - 2026
===========================================================
