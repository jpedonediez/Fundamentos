cree repositorio --> lo de gitignore es ambiente virtual para que git lo ignore, pq esto no tiene que estar en la entrega


cree el ambiente virtual --> venv

creo requirements.txt donde va a tener tods los paquetes instalados en mi venv con su version.
Sirve para que cualquiera puede reconstruir rxactamente mi ambiente y no tener pproblemas al ejecutarlo por diferentes versiones o no tener instalado ciertas cosas.
Entonces en el README (como parte de las instrucciones para la ejecucion vamos a tener que poner :

ejecutar:
    python3 m venv venv
    source venv/bin/activate
    pip install -r requirement.txt

logrando que se instalen todas las versiones indicadas en el ambiente virtual en el qeu se va a ejecutar nuestro tpe.


PAQUETES INSTALADOS Y QUE ESTAN EN REQUIREMENTS.TXT (cuales son, para que sirve, que hacen?)

-- paquetes de análisis de datos
pandas --> libreria para manipular datos tabulares (DataFrame, Series). Lo usamos para cargar el CSV (nuestra database está en este formato), limpiar, convertir tipos, agrupar, calcular describe(), contar nulos, get_dumies.

numpy --> cálculo numérico con arrays y matrices. Lo usamos para operacione vectorizadas, manejo de NaN, cálculos auxiliares. Además, pandas lo necesita y se apoya en este


-- paquetes de estadística

scipy --> Sirve para algoritmos científicos, su módulo scipy.stats tiene los test estadísticos.

statsmodels --> Modelos estadísticos con salida de tipo inferencial (tablas con p-valores, intervalos).

scikit-learn --> SIrve para machine learning.

-- paquetes de visualización

matplotlib --> líbreria base de gráficos en Python. La usamos para mostrar los histogramas, boxplots, scatter plots, QQ-plots, etc...

seaborn --> gráficos estadísticos de más alto nivel. Lo usamos para heatmap de corrlaciones, boxplots por grupos.


--paquetes de exploración

ydata-profiling --> genera reportes automáticos (ProfileReport) con histogramas nulos, correlaciones y alertas de cada variable. Lo usamos para que nos ayude con el análisis explorativo inicial

jupyterlab --> Sirve para los notebooks en el navegador. LO usamos para correr y escribir los notebooks.

ipykernel --> permite que Jupyter ejecuta código Python dentro de tu venv. Necesario para que el notebook encuentre su ambiente. Puente entre Jupytery Python en el ambiente virtual (venv)


IMPORTANTE CHEQUEAR QUE USEMOS TODOS LOS PAQUETES DEL requirements.txt ANTES DE ENTREGAR, SI NO USAMOS ALGUNO ==> LO ELIMINAMOS Y VOLVEMOS A HACER pip freeze > requirements.txt PARA QUE QUEDEN ACTUALIZADOS LOS PAQUETES/LIBRERIAS QUE SI UTILIZAMOS
