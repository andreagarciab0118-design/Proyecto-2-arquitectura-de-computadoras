Arquitectura de Computadoras I - II Semestre 2025

Instituto Tecnológico de Costa RicaDescripción GeneralEste proyecto implementa una unidad de punto flotante de media precisión (FP16) optimizada, diseñada para ser integrada en un procesador RISC-V mínimo. La unidad procesa operandos en paquetes de 32 bits que comprimen dos valores de punto flotante de 16 bits, permitiendo operaciones vectoriales compactas.El proyecto es parte de una investigación enfocada en especialización de hardware para aceleración de tareas específicas, con énfasis en diseño eficiente y sintetizable para FPGAs AMD Xilinx.Objetivos del ProyectoProblema 1: Integración con RISC-V

Integrar la unidad FP16 dentro de una implementación RISC-V mínima (RV32I)
Extender el ISA para soportar las nuevas instrucciones de punto flotante
Sintetizar e implementar el diseño completo en FPGA AMD Kria KV260
Caracterizar consumo de recursos (LUTs, BRAM, DSPs, Registros)
Medir frecuencia máxima de operación y latencia de instrucciones
Problema 2: Optimización con DSP
El proyecto incluye las siguientes mejoras sobre la implementación base:
Integración de celdas DSP48: Utilización de bloques DSP nativos de FPGA para operaciones aritméticas
Análisis comparativo: Contraste de recursos y frecuencia antes/después de DSP
Parametrización de buses: Configuración flexible del tamaño de registros de entrada
Precisión arbitraria: Parametrización de exponentes y mantisas más allá de IEEE 754
Exploración del espacio de diseño (DSE): Estudio de escalabilidad según parámetros (opcional)
Características TécnicasUnidad de Punto Flotante FP16

Formato de entrada: Paquetes de 32 bits con dos operandos FP16
Estándar: Compatible con IEEE 754 half-precision
Operaciones: Suma, resta, multiplicación (configurables)
Optimización: Uso de bloques DSP48 para eficiencia
Arquitectura RISC-V

ISA Base: RV32I
Extensiones: Instrucciones personalizadas para FP16
Implementación: Sintetizable para FPGA
Target: AMD Kria KV260 Vision AI Starter Kit
