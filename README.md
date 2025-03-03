# product-landing-page

La estructura semántica usada en mi proyecto es la siguiente:
`<body>`
`<header>`
`<main>`
`<footer>`

Siendo esta la estructura inicial de mi landing-page

El prompt que le dí a la IA para solicitar sugerencias de mejora en mi página fue esta:
Sigue estas indicaciones y mejora mi proyecto respetando la semántica y mejorandola de ser el caso. 
HU4: Footer con Información de Contacto “Como visitante, quiero encontrar fácilmente la información de contacto y enlaces importantes al final de la página, para poder comunicarme con la empresa o acceder a recursos adicionales.”

Criterios de Aceptación:
Email de contacto
Teléfono de soporte
Horarios de atención
Enlaces Importantes: Términos y condiciones
Redes sociales


Pude validar y por ello usar la respuestas que dió la IA debido a que si cumplia con los parametros que le solicite y también agregó estilos al css.


## Lab2:
Para este laboratorio las media queries usadas son ajustes para diferentes dispositivos

1024px → Tamaño ajustado para tablets y laptops pequeñas.

768px → Tamaño ajustado para tablets en vertical y móviles grandes.

480px → Tamaño ajustado para móviles pequeños.

```
/* Media Queries */

/* Pantallas de hasta 1024px (Tabletas y laptops pequeñas) */
@media (max-width: 1024px) {
  header nav {
    flex-direction: column;
    align-items: center;
  }
  header > nav > ul {
    gap: 16px;
  }
  #hero img {
    width: 300px;
  }
  #features {
    flex-direction: column;
    align-items: center;
  }
  .footer-container {
    flex-direction: column;
    align-items: center;
  }
}

/* Pantallas de hasta 768px (Tabletas en vertical y móviles grandes) */
@media (max-width: 768px) {
  header > nav > ul {
    flex-direction: column;
    text-align: center;
    gap: 10px;
  }
  #hero h1 {
    font-size: 36px;
  }
  #hero div p {
    font-size: 18px;
  }
  #features {
    gap: 20px;
  }
  #features > div {
    width: 100%;
    max-width: 400px;
  }
}

/* Pantallas de hasta 480px (Móviles pequeños) */
@media (max-width: 480px) {
  header nav {
    padding: 10px;
  }
  header > nav > ul {
    gap: 8px;
  }
  #hero {
    padding: 40px 10px;
  }
  #hero h1 {
    font-size: 28px;
  }
  #hero img {
    width: 250px;
  }
  #features {
    padding: 20px 10px;
  }
  #delivery, #payment-methods {
    padding: 20px 10px;
  }
}
```