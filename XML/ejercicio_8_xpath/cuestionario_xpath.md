# Cuestionario tipo test: XPath
Cuestionario progresivo sobre XPath, navegación por documentos XML, selección de elementos, uso de atributos y aplicación de predicados.

---

### 1. ¿Qué lenguaje se utiliza en la práctica para localizar información dentro de un documento XML?
- [x] **XPath** (Correcta)
- [ ] SQL
- [ ] CSS

### 2. Si queremos seleccionar todos los elementos `<rutina>` que están directamente bajo `<rutinas>`, ¿qué expresión XPath es adecuada?
- [ ] rutinas/rutina/rutinas
- [x] **/rutinas/rutina** (Correcta)
- [ ] /rutina/rutinas

### 3. Dado un elemento `<rutina>` que contiene `<nombre>` y `<nivel>`, ¿qué XPath permite seleccionar el elemento `<nombre>`?
- [ ] /nombre/rutina
- [ ] /rutina/nivel
- [x] **/rutina/nombre** (Correcta)

### 4. ¿Qué expresión XPath obtiene los elementos `<nivel>` de todas las rutinas?
- [ ] /rutinas/nivel/rutina
- [x] **/rutinas/rutina/nivel** (Correcta)
- [ ] /nivel/rutinas/rutina

### 5. ¿Qué significa el símbolo `/` en una expresión XPath?
- [x] **Permite avanzar de un nodo a otro siguiendo la estructura del árbol.** (Correcta)
- [ ] Permite acceder a un atributo.
- [ ] Permite establecer una condición.

### 6. Dado un elemento `<rutina>`, ¿qué expresión localiza la rutina cuyo atributo id vale RUT001?
- [x] **/rutina[@id='RUT001']** (Correcta)
- [ ] /rutina[id='RUT001']
- [ ] /rutina/id='RUT001'

### 7. ¿Qué símbolo se utiliza en XPath para acceder a un atributo?
- [x] **@** (Correcta)
- [ ] #
- [ ] $

### 8. Dado un documento con rutinas identificadas mediante el atributo id, ¿qué XPath selecciona únicamente la rutina RUT002?
- [ ] /rutinas/rutina[id='RUT002']
- [x] **/rutinas/rutina[@id='RUT002']** (Correcta)
- [ ] /rutinas/rutina[@RUT002='id']

### 9. ¿Qué función cumplen los corchetes `[]` en una expresión XPath?
- [ ] Permiten acceder directamente a un atributo.
- [ ] Permiten seleccionar siempre el primer elemento.
- [x] **Permiten aplicar una condición o filtro.** (Correcta)

### 10. ¿Qué XPath selecciona el nombre de la rutina cuyo atributo id es RUT001?
- [ ] /rutinas/rutina/nombre[@id='RUT001']
- [x] **/rutinas/rutina[@id='RUT001']/nombre** (Correcta)
- [ ] /rutinas/nombre/rutina[@id='RUT001']

### 11. Dado un elemento `<rutina>` con un hijo `<nivel>`, ¿qué XPath obtiene su elemento `<nivel>`?
- [x] **/rutina[@id='RUT002']/nivel** (Correcta)
- [ ] /rutina/nivel[@id='RUT002']
- [ ] /nivel/rutina[@id='RUT002']

### 12. ¿Qué expresión selecciona todos los elementos `<ejercicio>` de la rutina RUT001?
- [x] **/rutina[@id='RUT001']/ejercicios/ejercicio** (Correcta)
- [ ] /rutina/ejercicio[@id='RUT001']/ejercicios
- [ ] /ejercicios/rutina[@id='RUT001']/ejercicio

### 13. ¿Qué XPath obtiene los nombres de todos los ejercicios pertenecientes a la rutina RUT001?
- [ ] /rutina/nombre/ejercicios/ejercicio[@id='RUT001']
- [ ] /rutina[@id='RUT001']/nombre/ejercicio
- [x] **/rutina[@id='RUT001']/ejercicios/ejercicio/nombre** (Correcta)

### 14. ¿Qué expresión selecciona las rutinas cuyo elemento `<nivel>` contiene el texto Principiante?
- [ ] /rutinas/rutina[@nivel='Principiante']
- [x] **/rutinas/rutina[nivel='Principiante']** (Correcta)
- [ ] /rutinas/rutina/nivel='Principiante'

### 15. ¿Qué XPath obtiene los elementos `<nivel>` cuyo contenido sea Principiante?
- [ ] /rutinas/rutina[@nivel='Principiante']
- [x] **/rutinas/rutina[nivel='Principiante']/nivel** (Correcta)
- [ ] /rutinas/nivel[@Principiante]

### 16. ¿Qué XPath localiza el número de series del ejercicio Sentadilla dentro de RUT001?
- [x] **/rutina[@id='RUT001']/ejercicios/ejercicio[nombre='Sentadilla']/series** (Correcta)
- [ ] /rutina/series[@id='RUT001']/ejercicio[nombre='Sentadilla']
- [ ] /rutina[@id='RUT001']/ejercicios/series[ejercicio='Sentadilla']

### 17. ¿Qué XPath localiza las repeticiones del ejercicio Sentadilla dentro de RUT001?
- [ ] /rutina[@id='RUT001']/repeticiones/ejercicio[nombre='Sentadilla']
- [x] **/rutina[@id='RUT001']/ejercicios/ejercicio[nombre='Sentadilla']/repeticiones** (Correcta)
- [ ] /rutina/repeticiones[@id='RUT001']/nombre[.='Sentadilla']

### 18. ¿Qué XPath obtiene los nombres de los ejercicios pertenecientes únicamente a las rutinas de nivel Principiante?
- [ ] /rutinas/rutina/nivel='Principiante'/ejercicios/ejercicio/nombre
- [x] **/rutinas/rutina[nivel='Principiante']/ejercicios/ejercicio/nombre** (Correcta)
- [ ] /rutinas/rutina[@nivel='Principiante']/nombre/ejercicio

### 19. ¿Qué expresión localiza las series del ejercicio Remo con barra de RUT001?
- [x] **/rutina[@id='RUT001']/ejercicios/ejercicio[nombre='Remo con barra']/series** (Correcta)
- [ ] /rutina[@id='RUT001']/series/ejercicio[nombre='Remo con barra']
- [ ] /rutina/ejercicios/series[nombre='Remo con barra']/@id

### 20. ¿Cuál es la interpretación completa de `/rutinas/rutina[@id='RUT001']/ejercicios/ejercicio[nombre='Sentadilla']/repeticiones`?
- [x] **Busca todas las rutinas, selecciona RUT001, entra en sus ejercicios, localiza Sentadilla y obtiene sus repeticiones.** (Correcta)
- [ ] Busca una rutina cuyo elemento <repeticiones> tenga el atributo RUT001 y después busca Sentadilla.
- [ ] Busca todas las repeticiones del documento y comprueba posteriormente si pertenecen a Sentadilla.
