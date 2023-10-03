README

el Main.py tiene todas las funciones y el modelo de ML para la Api, no pude doplyar todo por falta de RAM, asi que solo hay 2 funciones funcionales en el deploy

El EDA lo realice despues de crear la Api, principalmente porque por mas informacion que pueda extraer de este los datos los corte con sierra para que entren en render asi que no iban a decir 100% lo mismo quiza

por otro lado el final del ETL es donde comienza El EDA y el notebook que dice 't' es donde prepare los dataset para la api, digamos que es como un quirofano medio criminal, esa parte no la retoque ni acomede el codigo que hay ahi es como se fue creando los df1 a df5 para el deploy

para explicar de forma sencilla esa parte voy a decir que reduje los dataframes a las columnas que necesitaba para crear las funciones, luego les hice merge creando un dataframe para cada funcion, despues los reduje, primero cambiando los tipos de datos a formatos mas ligeros ej: int64 a int 16 con el fin de disminuir el peso de los dataset para subir a github
luego cuando no me alcanzo con eso los reduje de manera aleatoria y borre nulos y duplicados
TODO este proceso pudo malograr la data pero al set para un MVP no lo vi de vital importancia por eso lo deje por separado

los datos que estan en parquet son para facilitar su exportacion a github ya que esa data esta mas limpia y menos malograda: me animaria a decir casi sana
 asi es como queda mi proyecto que voy a entregar al final:

 ETL la data limpia y sin malograr para hacer el EDA

 EDA un analisis de las relaciones de datos con principal enfasis en los generos de videojuegos, los precios , las empresas, las horas de juego, deje de lado en el EDA las relaciones con las reviews principalmente porque no me gusta como nltk trata los comentarios es MUY pesimista, luego en el EDA se nota que hubo un periodo donde faltan juegos y se ven varios outliers en el precio los que afectaron a la Media tambien, por eso la Moda y la Mediana dan parecido.

 Main aca estan las funciones y la Api para los 5 endpoints algunas se me desvirtuaron un poco pero son presentable creo

 t aca esta el proceso que use para crear los datasets que alimentarian a las api, estos no los subo porque no llego con el espacio y la velocidad de internet para que este listos al horario correspondiente asi que deje documentado el proceso
 
