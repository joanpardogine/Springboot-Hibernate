
## **1.** Instalació IntelliJ IDEA  

### **IntelliJ IDEA** – the **Leading Java** and Kotlin IDE
#### The **IDE** that makes development a more productive and enjoyable experience

<img src="./imatges/Mediamodifier-Design.svg" style="height:30px;"></img>
<!-- ![image](./imatges/Mediamodifier-Design.svg) -->

[**Download IntelliJ IDEA**](https://www.jetbrains.com/idea/download/)
* Community Edition
* The IDE for pure Java and Kotlin development

#### Copia aquest fitxer [**```ideaIC-2023.1.1.exe```**](./fitxers/ideaIC-2023.1.1.exe)
* Mida del fitxer ```633 MB (663.963.584 bytes)```

#### O fes servir aquest enllaç de descàrrega directe [Use the direct link **```ideaIC-2023.1.1.exe```**](https://download.jetbrains.com/idea/ideaIC-2023.1.1.exe?_gl=1*1k8vect*_ga*MTg2MTY5NjQ4LjE2Nzk5Mzk4Njc.*_ga_9J976DJZ68*MTY4Mjg3MzkwNy4yLjEuMTY4Mjg3Mzk0MC4yNy4wLjA.&_ga=2.48120163.554094189.1682873907-186169648.1679939867)

<summary>

## Instal·lació

<details>

### **1.** Executa el fitxer **```ideaIC-2023.1.1.exe```**.

![IntelliJ-IDEA_00001.png](./imatges/IntelliJ-IDEA_00001.png)
### **2.** Pitja el botó **següent** (<code> <b><u>N</u>ext ></b> </code>) per continuar,

![IntelliJ-IDEA_00002.png](./imatges/IntelliJ-IDEA_00002.png)
### **3.** No cal, però si vols pots modificar la ruta (<code> <b> B<u>r</u>owser...</b></code>), i si no, pitja el botó **següent** (<code> <b><u>N</u>ext ></b> </code>) per continuar,

![IntelliJ-IDEA_00003.png](./imatges/IntelliJ-IDEA_00003.png)
### **4.** Assegura't que estàn marcades les segünents opcions:

> #### **Create Desktop Shortcut**
> 
> - :white_check_mark: IntelliJ IDEA Community Edition
> 
> ####  **Update Context Menu**
> 
> - :white_check_mark: Add "Open Folder as Project"
>  
> ####  **Update ```PATH``` Variable (restart needed)**
> 
> - :white_check_mark: Add "**```bin```**" folder to the > **```PATH```**
> 
> ####  **Create associations**
> 
> - :white_check_mark: **```.java```**

Quan estiguin totes aquestes opcions marcades, pitja el botó **següent** (<code> <b><u>N</u>ext ></b> </code>) per continuar,

> ## **NOTA**: Pot ser que no estiguin exactament aquestes opcions!

![IntelliJ-IDEA_00004.png](./imatges/IntelliJ-IDEA_00004.png)

 pitja el botó **Install** (<code><b><u>I</u>nstall</b> </code>) per començar la instal·lació.
<!--  
![IntelliJ-IDEA_00005.png](./imatges/IntelliJ-IDEA_00005.png)

![IntelliJ-IDEA_00006.png](./imatges/IntelliJ-IDEA_00006.png) -->

![IntelliJ-IDEA_00007.png](./imatges/IntelliJ-IDEA_00007.png)

### **4.** Marca l'opció ***I want to manually reboot later***, i recorda que cal reiniciar l'equip abans de que funcioni la instal·lació:

> :radio_button: **```I want to manually reboot later```**

 i pitja el botó **Finish** (<code><b><u>F</u>inish</b> </code>) per començar la instal·lació.

![IntelliJ-IDEA_00008.png](./imatges/IntelliJ-IDEA_00008.png)


Si tot ha anat correctament, s'ha creat la següent icona a l'escriptori,

<img src="./imatges/IntelliJ-IDEA_exe_00008.png" height="100"></img>

i l'aplicació es troba a la següent carpeta:
```"C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2023.1.1\bin\idea64.exe"```

Abans d'obrir l'aplicació, recordem que cal reiniciar l'ordinador.
</details>
</summary>

Ja podem obrir l'aplicació **```IntelliJ IDEA```**

<img src="./imatges/IntelliJ-IDEA_exe_00008.png" height="100"></img>


Només començar, apareiex la següent finestra **IntelliJ IDEA User Agreement** (***Acord d'usuari d'IntelliJ IDEA***)

![IntelliJ-IDEA_exe_00009.png](./imatges/IntelliJ-IDEA_exe_00009.png)

Marquem l'opció **```I confirm that I have read and accept the terms of this User Agreement```** i pitjem el botó **següent** (<code> <b> Continue </b></code>) per continuar,


A continuació apareiex la finestra **Data sharing** (***Compartició de dades***)
El text que apareix diu:

> Ajudeu a JetBrains a millorar els seus productes enviant dades anònimes sobre les funcions i els connectors utilitzats, la configuració de maquinari i programari, estadístiques sobre tipus de fitxers, nombre de fitxers per projecte, etc. Tingueu en compte que això no inclourà dades personals ni cap informació sensible, com ara codi font, noms de fitxers, etc. Les dades enviades compleixen la Política de privadesa de JetBrains.

En aquest punt cadascú és lliure de compartir la seva informació o no.

Ara ja tenim l'aplicació oberta i funcionant correctament, amb la següent pantalla:

![IntelliJ-IDEA_exe_00011.png](./imatges/IntelliJ-IDEA_exe_00011.png)

En contra del que qualsevol pensaria, NO crearem el projecte des de l'opció New Project, ja que al crear un projecte genèric, el crea amb una estrucutgra molt reduïda, i nosaltres voldrem començar amb un projecte que ja cotingui una pila de llibreries que farem servir.

Per crear el nou projecte anirem a la ruta https://start.spring.io/

<a href="https://start.spring.io/"><span class="logo-content" tabindex="-1"><svg aria-hidden="true" focusable="false" data-icon="spring-initializr" role="img" xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" class="" viewBox="0 0 992.4 141.6"><g><path class="st0" d="M153.4,62.6l-30.2-52.3c-2.6-4.5-9.1-8.3-14.3-8.3H48.5c-5.2,0-11.7,3.7-14.3,8.3L4,62.6 c-2.6,4.5-2.6,12,0,16.5l30.2,52.3c2.6,4.5,9.1,8.3,14.3,8.3h60.4c5.2,0,11.7-3.7,14.3-8.3l30.2-52.3 C156.1,74.5,156.1,67.1,153.4,62.6z"></path><g><circle class="st1" cx="36.7" cy="115.2" r="6.1"></circle></g><g><path class="st1" d="M139,97.4C121.3,121,83.5,113,59.3,114.2c0,0-4.3,0.2-8.6,0.9c0,0,1.6-0.7,3.7-1.4c17-5.9,25-7.1,35.4-12.4 c19.4-9.9,38.7-31.6,42.7-54.1c-7.4,21.6-29.9,40.3-50.3,47.8c-14,5.2-39.3,10.2-39.3,10.2l-1-0.5C24.5,96.4,24,59,55.3,47 C69,41.7,82.2,44.6,97,41.1c15.8-3.8,34.1-15.6,41.6-31.1C146.9,34.8,156.9,73.5,139,97.4z"></path><path class="st0" d="M138.6,10c8.3,24.8,18.4,63.5,0.4,87.4c-11.1,14.8-30.1,17.2-48.7,17.2c-8.8,0-17.5-0.5-25.2-0.5 c-2,0-3.9,0-5.7,0.1c0,0-4.3,0.2-8.6,0.9c0,0,1.6-0.7,3.7-1.4c17-5.9,25-7.1,35.4-12.4c19.4-9.9,38.7-31.6,42.7-54.1 c-7.4,21.6-29.9,40.3-50.3,47.8c-14,5.2-39.3,10.2-39.3,10.2l0,0l-1-0.5C24.5,96.4,24,59,55.3,47C69,41.7,82.2,44.6,97,41.1 C112.8,37.4,131.1,25.5,138.6,10 M139.1,2.1l-3.2,6.6c-7.5,15.6-25.8,26.2-39.6,29.5C90.1,39.7,84,40,78.2,40.3 c-7.7,0.4-15.7,0.8-23.9,3.9C35,51.6,27.6,67.8,27.1,80.5c-0.5,12.1,4.7,22.6,13.2,26.9c0.5,0.3,1.6,0.9,2.5,0.9h1.3l0.2-0.2 c5.8-1.2,26.5-5.6,38.9-10.1c8.6-3.2,18.3-8.6,27.1-15.8c-6.5,6.9-14.1,12.7-21.8,16.6c-6.3,3.2-11.7,4.9-19.2,7.2 c-4.4,1.3-9.5,2.9-15.7,5c-2.2,0.7-3.8,1.5-3.9,1.5l-2.2,4.5l3.9,1.2c4.1-0.7,8.2-0.9,8.3-0.9c1.7-0.1,3.5-0.1,5.5-0.1 c3.7,0,7.6,0.1,11.7,0.3c4.4,0.1,8.9,0.3,13.5,0.3c18.5,0,39-2.2,51.1-18.4c14.1-18.8,14.2-48.3,0.1-90.2L139.1,2.1L139.1,2.1z"></path></g></g><g><g><path class="st0" d="M194.1,98.2c-1.5-0.8-2.5-2.5-2.5-4.7c0-3,2.4-5.5,5.5-5.5c1.1,0,2.1,0.4,2.9,0.8c5.7,3.8,11.7,5.7,17,5.7 c5.8,0,9.2-2.5,9.2-6.4v-0.3c0-4.7-6.3-6.2-13.2-8.3c-8.7-2.5-18.5-6-18.5-17.3v-0.3c0-11.2,9.3-18,21-18c6.3,0,12.8,1.8,18.6,4.8 c1.9,1,3.3,2.8,3.3,5.2c0,3.1-2.5,5.5-5.7,5.5c-1.1,0-1.8-0.3-2.6-0.6c-4.8-2.5-9.7-4-13.8-4c-5.3,0-8.3,2.5-8.3,5.8v0.3 c0,4.4,6.4,6.2,13.3,8.4c8.7,2.6,18.4,6.7,18.4,17.2v0.3c0,12.4-9.7,18.6-21.9,18.6C209,105.2,200.9,102.8,194.1,98.2z"></path><path class="st0" d="M243.6,50.8c0-3.8,2.9-6.8,6.7-6.8c3.8,0,6.8,3,6.8,6.8v4c4.4-6.2,10.6-11.1,20.1-11.1 c13.8,0,27.4,10.9,27.4,30.7v0.3c0,19.6-13.5,30.7-27.4,30.7c-9.8,0-16-4.9-20.1-10.4v20.9c0,3.8-3,6.8-6.8,6.8 c-3.6,0-6.7-2.9-6.7-6.8V50.8z M291,74.7v-0.3c0-11.4-7.7-18.9-16.8-18.9c-9.2,0-17.2,7.7-17.2,18.9v0.3c0,11.3,8,18.9,17.2,18.9 C283.3,93.7,291,86.4,291,74.7z"></path><path class="st0" d="M309.8,50.8c0-3.8,2.9-6.8,6.7-6.8s6.8,3,6.8,6.8v3.3c0.6-5,8.9-10.1,14.8-10.1c4.3,0,6.7,2.8,6.7,6.7 c0,3.5-2.4,5.9-5.4,6.5c-9.7,1.6-16.2,10.1-16.2,21.7v19.5c0,3.6-3,6.7-6.8,6.7c-3.6,0-6.7-2.9-6.7-6.7V50.8L309.8,50.8 L309.8,50.8z"></path><path class="st0" d="M350.2,50.9c0-3.8,2.9-6.8,6.7-6.8s6.8,3,6.8,6.8v47.6c0,3.8-3,6.7-6.8,6.7c-3.6,0-6.7-2.9-6.7-6.7V50.9z"></path><path class="st0" d="M370.6,50.9c0-3.8,2.9-6.8,6.7-6.8c3.8,0,6.8,3,6.8,6.8v2.8c3.8-5.5,9.3-9.7,18.5-9.7c13.3,0,21,8.9,21,22.6 v31.8c0,3.8-2.9,6.7-6.7,6.7s-6.8-2.9-6.8-6.7V70.8c0-9.2-4.5-14.5-12.7-14.5c-7.8,0-13.3,5.5-13.3,14.7v27.5c0,3.8-3,6.7-6.8,6.7 c-3.6,0-6.7-2.9-6.7-6.7L370.6,50.9L370.6,50.9z"></path><path class="st0" d="M483.1,43.9c-3.8,0-6.8,3-6.8,6.8v4c-4.4-6.2-10.6-11.1-20.1-11.1c-13.8,0-27.4,10.9-27.4,30.7v0.3 c0,19.6,13.5,30.7,27.4,30.7c9.8,0,16-4.9,20.1-10.3c-0.6,10.7-7.2,16.2-18.6,16.2c-6.8,0-12.7-1.6-18.1-4.7 c-0.6-0.4-1.5-0.5-2.4-0.5c-3.1,0-5.8,2.5-5.8,5.5c0,2.6,1.5,4.5,3.8,5.4c7.2,3.5,14.6,5.3,22.9,5.3c10.7,0,19-2.5,24.3-7.9 c4.9-4.9,7.5-12.3,7.5-22.2V50.8C489.8,46.9,486.8,43.9,483.1,43.9z M459.3,93.5c-9.3,0-16.8-7.3-16.8-19v-0.3 c0-11.4,7.7-18.9,16.8-18.9c9.2,0,17.2,7.7,17.2,18.9v0.3C476.6,85.9,468.6,93.5,459.3,93.5z"></path><path class="st0" d="M363.8,27.8c0,3.8-3,6.8-6.8,6.8s-6.8-3-6.8-6.8s3-6.8,6.8-6.8C360.6,20.9,363.8,23.9,363.8,27.8z"></path></g><g><path class="st0" d="M505.3,58.1c-3.8,0-6.9-3.1-6.9-6.9c0-3.9,3.1-6.9,6.9-6.9c3.9,0,6.9,3.1,6.9,6.9 C512.2,55,509.2,58.1,505.3,58.1z M505.3,45.3c-3.3,0-5.9,2.6-5.9,5.9c0,3.3,2.6,5.9,5.9,5.9c3.3,0,5.9-2.6,5.9-5.9 C511.2,47.8,508.6,45.3,505.3,45.3z M507.2,55.1l-2-3.1h-1.4v3.1h-1.1v-7.9h3.3c1.4,0,2.6,1,2.6,2.4c0,1.8-1.6,2.4-2,2.4l2.1,3.1 L507.2,55.1L507.2,55.1z M505.8,48.2h-2v2.8h2.1c0.6,0,1.4-0.5,1.4-1.4C507.3,48.7,506.6,48.2,505.8,48.2z"></path></g></g><g><path fill="currentColor" d="M529.9,27.2c0-4.4,3.6-8.1,8.2-8.1c4.5,0,8.1,3.8,8.1,8.1c0,4.4-3.6,8.2-8.1,8.2C533.6,35.5,529.9,31.6,529.9,27.2z M530.9,44.7h14.4v60.8h-14.4V44.7z"></path><path fill="currentColor" d="M616.9,66.8v38.7H603V69.6c0-8.2-5.3-14.1-12.8-14.1c-7.5,0-13.8,5.1-14.7,11.5v38.5h-14.4V44.7h14.4v8.1 c3.8-5.6,10.8-9.5,18.8-9.5C607.6,43.2,616.9,53,616.9,66.8z"></path><path fill="currentColor" d="M631.5,27.2c0-4.4,3.6-8.1,8.2-8.1c4.5,0,8.1,3.8,8.1,8.1c0,4.4-3.6,8.2-8.1,8.2C635.1,35.5,631.5,31.6,631.5,27.2z M632.4,44.7h14.4v60.8h-14.4V44.7z"></path><path fill="currentColor" d="M697.1,102.1c-3.4,2.9-8.4,4.8-12.9,4.8c-10.1,0-17.2-7.3-17.2-17.5V56.5h-8.8V44.7h8.8V27.9h14v16.7h13.8v11.9H681v31.1 c0,4.1,2.6,7.1,6,7.1c2.5,0,4.7-0.9,6-2.2L697.1,102.1z"></path><path fill="currentColor" d="M707.4,27.2c0-4.4,3.6-8.1,8.2-8.1c4.5,0,8.1,3.8,8.1,8.1c0,4.4-3.6,8.2-8.1,8.2C711,35.5,707.4,31.6,707.4,27.2z M708.3,44.7h14.4v60.8h-14.4V44.7z"></path><path fill="currentColor" d="M791.2,68.9v36.6h-14v-7.3c-4.5,5.6-12.1,8.7-19.2,8.7c-12.9,0-22.7-7.6-22.7-19.4c0-12,11.2-20.2,24.8-20.2 c5.5,0,11.5,1.2,17.1,3.3v-1.6c0-7.1-3.9-13.9-14.9-13.9c-5.8,0-11.3,2-16.5,4.6l-4.9-10c8.6-4.2,16.6-6.4,24.2-6.4 C781.2,43.2,791.2,53.5,791.2,68.9z M777.2,86.4v-6.8c-4.5-1.5-9.5-2.4-14.9-2.4c-7.2,0-12.9,4-12.9,9.8c0,5.8,5.1,9.4,11.9,9.4 C768.1,96.4,775.5,92.9,777.2,86.4z"></path><path d="M806.7,23.2h14.4v82.3h-14.4V23.2z" fill="currentColor"></path><path fill="currentColor" d="M836,27.2c0-4.4,3.6-8.1,8.2-8.1c4.5,0,8.1,3.8,8.1,8.1c0,4.4-3.6,8.2-8.1,8.2C839.6,35.5,836,31.6,836,27.2z M836.9,44.7 h14.4v60.8h-14.4V44.7z"></path><path fill="currentColor" d="M864.7,95L897,57.2h-31.5V44.7h50.5l-0.1,10.5l-32.4,37.8h32.7v12.6h-51.4V95z"></path><path fill="currentColor" d="M965.6,43.2v12.2c-13.1,0-21.8,7.8-21.8,19.3v30.7h-14.4V44.7h14.4v11.8C947.7,48.3,955.6,43.2,965.6,43.2z"></path></g></svg></span></a>


# Curso-de-Springboot-Hibernate
Curso de Java Fullstack (Springboot, Hibernate y JWT Session)

Si tienes interés en dominar Java Web Services con Spring Boot o en desarrollar API RestFUL a nivel empresarial, Udemy tiene un curso para ti.

Acceso al Curso completo: https://www.youtube.com/watch?v=7vHzVN0EiQc

Ayúdame a seguir creciendo, te invito a suscribirte: 

👉 Youtube: http://bit.ly/LucasMoy


Puedes encontrarme también en:

🔹 Instagram: https://www.instagram.com/lucasmoy.dev/

🔹 Facebook: https://www.fb.com/lucasmoy.dev/

🔹 Twitter: https://twitter.com/lucasmoy_dev/

