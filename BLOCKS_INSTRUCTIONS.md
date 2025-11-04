Bloques esenciales para Kodular:
- Variables globales: dbUrl, apiKey, userId, idToken, idioma, listaAfirmaciones
- Screen1.Initialize: detect language, anonymous sign-in, load messages
- Chat flow: btnSend -> moderate -> POST to Realtime DB /usuarios/<userId>/mensajes.json?auth=<idToken>
- Load messages: Web_DB.Get from /usuarios/<userId>/mensajes.json?auth=<idToken>
- Quick replies on Home: use mensajes_multileng.quickReplies[idioma]
- Exercise breathing: TTS + Clock timers
