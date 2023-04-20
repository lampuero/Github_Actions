# Github_Actions
Test repository for github actions
## Test 1
- Prueba de automaton para revisar branch utilizara en checkout.
### Resultado
- No corrio.
## Test 2
- Se actualizo automaton ante falla en test 1 (cambio branch en pull_request_target).
### Resultado
- Corrio pero fallo.
## Test 3
- Se actualizo el comando ejecutado en run.
### Resultado
- Corrio bien.
## Test 4
- Se agrego comandos para imprimir titulo y cuerpo de pull request.
- Se agrego condicion para correr solo cuando la head branch empieza con `release/`.
### Resultado
- Fallo, al parecer los comandos para imprimir los datos del pr estaban mal.
## Test 5
- Se modificaron los comandos para imprimir datos pr.
- Se encerro condicion en parentesis
### Resultado
- Fallo
## Test 6
- Se corriogio un tipeo.
- Se volvio a condicion anterior
### Resultado
- Fallo
## Test 7
- Se indentifico y corrigio error que hizo que fallaran los test anteriores.
### Resultado
- Corrio bien
## Test 8
- Se volvio a agregar comandos a probar.
### Resultado
- Fallo al imprimir el body
## Test 9
- Se agrego condicion de nombre de head branch.
### Resultado
- Tal como se esperaba no se realizo el trabajo
## Test 10
- Mismo que test 9 pero ahora con el nombre correcto en head branch
### Resultado
- Corrio como se esperaba
## Test 11
- Se modifico el comando para imprimir cuerpo pr
### Resultado
- Fallo
## Test 12
- Se agrego comandos para imprimir variables disponibles.
### Resultado
- Funciono bien, se identifico que se fallo antes al imprimir el cuerpo del pr porque parte del texto era interpretado como un comando en vez de ser solo string. Solucion encerrar la variable en comillas.

## Test 13
- se agrego acciones para guardar en cache los pods
### Resultado
- El cache no se guarda porque el trabajo termina con errores.
## Test 14
- Se elimino el step que fallaba
