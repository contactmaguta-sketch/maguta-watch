# Maguta Watch AI — version propre avec Netlify Functions

IMPORTANT : cette version utilise une Netlify Function. Elle ne doit PAS être déployée par simple drag & drop si Netlify ne détecte pas les fonctions.

Méthode recommandée : connecter ce dossier à GitHub puis connecter le repo à Netlify.

Variables Netlify nécessaires :

OPENAI_API_KEY = votre clé OpenAI
OPENAI_MODEL = gpt-4.1-mini
EMAILJS_PUBLIC_KEY = 3jMz3yanN1aIue4wyo1je
EMAILJS_SERVICE_ID = service_mnzrb2s
EMAILJS_REPORT_TEMPLATE_ID = template_2uyu893
EMAILJS_ADMIN_TEMPLATE_ID = template_2uyu893
EMAILJS_CONFIRMATION_TEMPLATE_ID = template_2uyu893
ADMIN_EMAIL = contactmaguta@gmail.com

Dans EmailJS, le template utilisé doit contenir :
To Email: {{to_email}}
Subject: {{subject}}
Content: {{message}}

Après déploiement, tester :
https://votre-site.netlify.app/.netlify/functions/generate-and-send
Doit répondre Method not allowed en GET, ce qui prouve que la fonction existe.
