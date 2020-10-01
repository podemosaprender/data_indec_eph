# data_indec_eph

Encuesta Permanente de Hogares EPH INDEC Argentina en texto separado ej. para usar en Google Colab y otras herramientas de ciencia de datos.

Se tomaron los archivos disponibles desde 2003. Se alinearon las columnas para que se puedan concatenar todos. Se eliminaron las notas repetidas.

~~~
import pandas as pd
EphUrlPfx= 'http://www.podemosaprender.org/data_indec_eph/' #U: prefijo URL para obtener datos
df= pd.read_csv(EphUrlPfx+'hogar/hogar_a15t1.tsv.gz', sep='\t') 
#U: pandas puede leer directamente separado por tabuladores y comprimido con gzip desde una url
#U: los archivos disponibles se pueden ver en el repo, hay "hogar", "indiv" y "notas" 
# con a(año dos digitos)t(nro trimestre) donde el primer trimestre es 1

df.head()
~~~

[Aquí](https://github.com/podemosaprender/data_indec_eph/blob/master/ejemplos/eph_tutorial_0.ipynb) se puede ver un ejemplo completo, y probarlo en Colab

## Próximos pasos

Links a metodología e interpretación, se podrían agregar ejemplos Python/Colab y contribuir por ej. a https://diegokoz.github.io/Curso_R_EPH_clases/





ASK: dev@mauriciocap.com
