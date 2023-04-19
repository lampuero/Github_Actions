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
