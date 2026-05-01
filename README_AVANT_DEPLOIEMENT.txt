AVANT DEPLOIEMENT

1. Ouvre config.js
2. Remplace PASTE_YOUR_NEW_OPENAI_KEY_HERE par ta NOUVELLE clé OpenAI.
3. Sauvegarde.
4. Zippe index.html + success.html + config.js ensemble.
5. Déploie le ZIP sur Netlify.

Cette version n’utilise PAS Netlify Functions, PAS Resend, PAS DNS.
Elle appelle OpenAI directement depuis le navigateur. C’est rapide pour tester, mais la clé OpenAI est visible dans le code source. A sécuriser plus tard avec un backend.
