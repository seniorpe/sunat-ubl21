# SUNAT - UBL 2.1
Para emitir documentos electrónicos SUNAT publica los archivos xsd basado en la estructura de UBL (Universal Business Language) en la versión 2.1.

Para poder usarlo se debe convertir en una librería de clases, para generar el archivo de clases se realiza con estos simple pasos:

- Ubicar la aplicación **xsd.exe**.
	> Ir a: C:\Program Files (x86)\Microsoft SDKs\Windows\v10.0A\bin\NETFX 4.8 Tools

- Abrir la consola de comandos y ejecutar el siguiente comando.
	> **xsd** D:\UBL21\maindoc\UBL-Invoice-2.1.xsd D:\UBL21\common\UBL-CommonExtensionComponents-2.1.xsd D:\UBL21\common\UBL-UnqualifiedDataTypes-2.1.xsd D:\UBL21\common\UBL-CommonBasicComponents-2.1.xsd D:\UBL21\common\UBL-CommonAggregateComponents-2.1.xsd D:\UBL21\common\UBL-QualifiedDatatypes-2.1.xsd D:\UBL21\common\CCTS_CCT_SchemaModule-2.1.xsd /c /n:Sunat.UBL21 /l:cs /o:D:\UBL21
