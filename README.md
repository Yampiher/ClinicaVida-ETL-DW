# ETL SSIS - Clinica Vida Plus

## Como ejecutar en otro PC
1. **Modo 32 bits (obligatorio para Excel):** Abrir `ClinicaVida_ETL_DatosNuevos.sln` en Visual Studio -> clic derecho en el proyecto -> **Propiedades** -> **Depuracion** -> cambiar `Run64BitRuntime` a `False`.
2. **Conexiones:** En la barra inferior de conexiones de `01_Cargar_STG.dtsx` y `02_Transformar_STG.dtsx`, apuntar los origenes Excel a sus archivos locales y el destino OLE DB a su instancia local de SQL Server (`.` o `localhost`).
3. **Ejecucion:** Ejecutar `01_Cargar_STG.dtsx` con `F5` y luego `02_Transformar_STG.dtsx` con `F5`.
