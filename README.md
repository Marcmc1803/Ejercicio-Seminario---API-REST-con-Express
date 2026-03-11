🚀 Projecte: Gestió de Relacions 1:N amb Mongoose Virtuals
Aquesta entrega se centra en l'evolució de l'API per gestionar una relació 1:N entre Organitzacions i Usuaris mitjançant l'Opció B: Virtuals, prioritzant l'escalabilitat i el rendiment.

🛠️ Implementació Tècnica
Mongoose Virtuals: S'ha definit la relació al model d'Organització com un camp virtual. Això evita redundàncies a la base de dades i facilita la gestió de dades relacionades.

Service Layer: Tota la lògica de Mongoose s'ha extret dels controladors. S'utilitza .populate() per carregar els usuaris i .lean() per retornar objectes JavaScript plans, millorant la velocitat de l'API.

Nou Endpoint & Swagger: S'ha creat la ruta GET /organizations/:id/users, verificada i documentada completament amb Swagger (OpenAPI).

Borrat en Cascada: S'ha programat un middleware pre-delete que elimina automàticament els usuaris associats quan s'esborra una organització.

🤖 Ús d'IA
Per al desenvolupament d'aquest projecte s'ha utilitzat una IA com a eina de suport. Ha estat d'ajuda per redactar els comentaris tècnics del codi, estructurar correctament les anotacions de Swagger i optimitzar la lògica del middleware de borrat per evitar conflictes amb els tipus de TypeScript.

📺 Explicació i Demo
En aquest vídeo es detalla la configuració dels Virtuals i es mostra el funcionament del sistema: https://youtu.be/kTjRwfctDQ4

