# supervised_learning_machine_learning

## Introdución 

La empresa Zyfra desarrolla soluciones de eficiencia para la industria pesada, crearemos un modelo para predecir la cantidad de oro extraído del mineral de oro.

Con este modelo ayudaremos a optimizar la producción y a eliminar parámetros no rentables

## conclusiones

- Los datos para el calculo de recuperación los tomamos del diagrama en la introducción
- El AEM del calculo de recuperación es muy cercano a 0, esto quiere decir que el calculo de recuperación es correcto
- Las columnas que no se encuentran el en conjunto de prueba son las columnas de:
	- características finales
	- purificación primaria
	- flotación
	- purificación secundaria
	- Columnas objetivo
- Los valores ausentes del DataFrame train, están distribuidos en todas la mayoría de las columnas
- Los valores ausentes del DataFrame test, son menores que test y solo se distribuyen en 5 columnas
- Los valores ausentes del DataFrame full, están distribuidos en todas la mayoría de las columnas
- Se puede observar que el cambio en Au (Oro) aumenta el numero de partículas después del proceso de primario de purificación
- Se puede observar que el cambio en Ag (Plata) disminuye el numero de partículas después del proceso de primario de purificación
- Se puede observar que el cambio en Pb (Plomo) se conservo el numero de partículas después del proceso de primario de purificación
- Se puede observar que la distribución de las partículas no varían significativamente en el conjunto de entrenamiento ni en el de prueba
- Se puede observar que en las tres etapas de cada material hay valores atípicos muy cercanos a 0, no eliminaremos datos, ya que los tres data frame tienen valores similares
- Se recomienda utilizar el modelo de Decision Tree Tegressor, ya que es el que menor sMAPE nos representa con las predicciones
- Se entrena el modelo Decision Tree Regressor con los datos de test, nos da un 12.8% de error en las predicciones
