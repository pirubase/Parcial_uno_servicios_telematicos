# Parcial_uno_servicios_telematicos
este es el github del primer parcial

*PRIMERA PARTE:*


1. Configuración del servidor maestro (192.168.50.3)

 Archivos modificados:
 - /etc/bind/named.conf.local
   

<img width="567" height="412" alt="image" src="https://github.com/user-attachments/assets/442098e4-414f-49e9-ac06-31684a933fa8" />

- /etc/bind/db.empresa.local
  

<img width="628" height="487" alt="image" src="https://github.com/user-attachments/assets/3ca3befb-7615-432c-b2ff-b65abbde5799" />


- /etc/bind/db.192
  

   <img width="623" height="417" alt="image" src="https://github.com/user-attachments/assets/01b2ee9d-84c1-4230-a916-1f61105b8647" />


2. Configuración del servidor esclavo (192.168.50.4)


- /etc/bind/named.conf.local
  

  <img width="666" height="343" alt="image" src="https://github.com/user-attachments/assets/ac111403-8767-48ac-90e0-f80fefbadb4f" />

  <img width="915" height="185" alt="image" src="https://github.com/user-attachments/assets/c0215569-8656-4806-9849-1a20c4daf1ff" />
  

3. Validación desde el cliente (192.168.50.2)

<img width="1032" height="680" alt="image" src="https://github.com/user-attachments/assets/e4c61294-4912-4581-84b3-de4a60e6b130" />


*SEGUNDA PARTE:*


1. Instalar y configurar Apache

<img width="386" height="66" alt="image" src="https://github.com/user-attachments/assets/c2ee8555-1f62-4aa7-be8f-d00f08be5c66" />

2. Habilitar el módulo mod_deflate

   <img width="363" height="73" alt="image" src="https://github.com/user-attachments/assets/e0e7c05e-1098-4ecc-8e58-e83db1b982fd" />


3. Configurar reglas específicas en Apache


<img width="555" height="77" alt="image" src="https://github.com/user-attachments/assets/221d2868-5b8f-4b7b-86ee-42534383a7a8" />

<img width="1458" height="272" alt="image" src="https://github.com/user-attachments/assets/39c0452c-ecbd-443d-92c1-395e8b8b7b7c" />

4. Configuración del servidor DNS local

<img width="468" height="133" alt="image" src="https://github.com/user-attachments/assets/bc2ed3a8-d91f-4c03-8178-972f34dff6b8" />

<img width="942" height="337" alt="image" src="https://github.com/user-attachments/assets/b1a57978-575e-4baf-b7b3-eb441d830412" />

<img width="718" height="95" alt="image" src="https://github.com/user-attachments/assets/c062ccd6-b800-4429-96e8-a32f61af3e83" />

5. Probar acceso desde diferentes clientes

<img width="1160" height="277" alt="image" src="https://github.com/user-attachments/assets/0936328b-fd2e-497c-a3d7-eed96338b2ee" />

<img width="1327" height="161" alt="image" src="https://github.com/user-attachments/assets/9435c9fa-62ca-4449-b0f3-5badac831a0f" />

*TERCERA PARTE:*


1. Instalar Ngrok


<img width="407" height="90" alt="image" src="https://github.com/user-attachments/assets/f2b195c6-0cc9-481c-a4c6-91be4106566e" />

<img width="723" height="62" alt="image" src="https://github.com/user-attachments/assets/983b9936-4c3b-4be5-9d91-312160297335" />

<img width="432" height="72" alt="image" src="https://github.com/user-attachments/assets/a39d8476-a8c5-4a86-b826-e8221bf9edbc" />

<img width="367" height="76" alt="image" src="https://github.com/user-attachments/assets/1d382f62-8a95-4ef3-b364-a7905cafa48a" />

2. Obtener y configurar el Authtoken

Creamos una cuenta gratuita en https://ngrok.com

En el dashboard de Ngrok copiamos nuestro authtoken.

<img width="1641" height="643" alt="image" src="https://github.com/user-attachments/assets/44debb00-035f-450a-b4ba-d5a422a4ca82" />

Lo registramos en la máquina servidor:


<img width="1242" height="53" alt="image" src="https://github.com/user-attachments/assets/2ae6dcef-1890-4958-9a3c-ed207e90b22c" />


3. Crear un túnel con Ngrok

<img width="1195" height="386" alt="image" src="https://github.com/user-attachments/assets/3f7c9005-3dfc-46ce-aef2-ae4f3ed8fd36" />

<img width="1002" height="847" alt="image" src="https://github.com/user-attachments/assets/502b99ba-8dce-4539-97b5-fdb65cd2641e" />
