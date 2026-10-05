# abrir-correo

Una sola página estática que abre la app de correo del móvil con un mensaje ya escrito.

Existe porque algunas aplicaciones de mensajería solo permiten enlaces `https` en sus botones y
rechazan `mailto:` y los enlaces propios de las apps de correo. El botón apunta aquí y esta
página hace el salto:

- iPhone: abre la app de Gmail (`googlegmail://`), con `mailto:` como alternativa.
- Android: `mailto:`, que el móvil entrega a su app de correo.
- Ordenador: Gmail en la web.

## Uso

```
https://doctorcako.github.io/abrir-correo/#to=<destinatario>&su=<asunto>&body=<mensaje>
```

Los tres valores van codificados como en cualquier URL. Viajan tras la almohadilla, la parte de
la dirección que el navegador no envía al servidor: esta página no recibe ni guarda ningún
mensaje, todo ocurre en el móvil de quien la abre.
