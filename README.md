# PPS-Unidad3Actividad28-AdrianCurtoSanchez

## Obtener InsecureBankv2

Podemos descargar el `apk` y el servidor de la URL https://github.com/dineshshetty/Android-InsecureBankv2/releases/tag/2.3.1

## Emular un dispositivo móvil en Genymotion

Pinchamos en el botón `create`.

![imagen](https://github.com/user-attachments/assets/19e9f1c5-0e41-448e-97aa-150683d44a9d)

Seleccionamos por ejemplo Pixel 2 y pinchamos en next.

![imagen](https://github.com/user-attachments/assets/60d1898b-c299-4fe4-877f-317aedb45b2d)

Dejamos las opciones por defecto y pinchamos en next.

![imagen](https://github.com/user-attachments/assets/aabed41d-4a66-412c-9fd0-935eb9b04c51)

![imagen](https://github.com/user-attachments/assets/61712237-260f-4384-bbee-602b1bb1e0ae)

![imagen](https://github.com/user-attachments/assets/40085db4-16df-4b09-815e-2c17a8387e7e)

![imagen](https://github.com/user-attachments/assets/f9a76108-ee6a-4a4a-96d7-c5332d84f260)

En las opciones de hipervisor debemos seleccionar "Network mode" de tipo "Bridge" y pinchamos en install.

![imagen](https://github.com/user-attachments/assets/82787bea-c0ec-4bb5-9de1-d7d2d233550a)

Para ejecutar la emulación solo tenemos que pulsar en el botón de play.

![imagen](https://github.com/user-attachments/assets/5950c22b-fb58-42ea-badd-ecda6847a761)

Y ya tenemos listo el emulador.

![imagen](https://github.com/user-attachments/assets/56e95773-12ac-4c09-a074-1bcb12ebb6da)

## Instalar apk en el emulador

Para instalar la aplicación en el emulador basta con arrastrar y soltar el apk de la aplicación al emulador. Ignoramos el mensaje que nos muestra.

![imagen](https://github.com/user-attachments/assets/d4e3459a-20b4-4768-82f0-d6fd1b55d869)

## Instalar MobSF

Desde la terminal de Docker decktop ejecutamos el siguiente comando que ejecutará el container de MobSF:
```
docker run -it --rm -p 8000:8000 -e MOBSF_ANALYZER_IDENTIFIER=10.0.3.250:5555 opensecurity/mobile-security-framework-mobsf:latest
```

![imagen](https://github.com/user-attachments/assets/a71d8acf-a62e-4d90-8ae8-3ebf3e292a34)

Y accedemos a la aplicación a través del navegador con la URL http://localhost:8000/login/?next=/ y las credenciales `mobsf:mobsf`.

## Análisis dinámico de la aplicación

Una vez dentro de MobSF en la URL http://localhost:8000 pinchamos en Dynamic Analyzer.

![imagen](https://github.com/user-attachments/assets/e4ccbd41-fb99-4b21-9cb5-bbd5cebbbc16)

Seleccionamos la opción de Android Dinamic Analyzer.

![imagen](https://github.com/user-attachments/assets/46f3ef38-0752-4092-ba46-e6e1bea9413c)

Vemos que ha detectado el emulador perfectamente, al abrir la aplicación a analizar deberá detectarla.






















