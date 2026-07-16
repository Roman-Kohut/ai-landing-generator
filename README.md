# 🪄 AI Generátor landing stránok

Nástroj, ktorý na základe krátkeho opisu biznisu vygeneruje pomocou AI **3 rôzne hotové návrhy jednostránkovej webstránky** (odvážny/moderný, minimalistický/elegantný, vrelý/priateľský štýl) — s textami, farbami aj štruktúrou prispôsobenými presne danému biznisu. Výsledok sa dá priamo v prehliadači upravovať (klikni na text a preprac ho) a stiahnuť ako hotový `.html` súbor.

## Ako to funguje

1. Opíšeš svoj biznis jednou-dvomi vetami (napr. *"kaviareň v Trnave, remeselná káva, útulná atmosféra"*)
2. AI vygeneruje **3 varianty** stránky súčasne, každý v inom vizuálnom štýle
3. Prepínaš medzi variantmi, vieš prepnúť náhľad mobil/desktop
4. Ktorúkoľvek časť textu vieš priamo upraviť kliknutím (režim "Upraviť text")
5. Ktorúkoľvek sekciu (hero, služby, referencie...) vieš nechať AI pregenerovať znova, ak sa ti nepáči
6. Stiahneš si hotovú stránku ako samostatný `.html` súbor, alebo skopíruješ kód

## Tech stack

- **React** (cez CDN, bez build kroku — beží priamo v prehliadači vďaka Babel Standalone)
- **Tailwind CSS** (cez CDN)
- **Groq API** (`openai/gpt-oss-120b`) pre generovanie obsahu a farebných tém

## Spustenie

Stačí otvoriť `index.html` v prehliadači (lokálne, alebo cez GitHub Pages — žiadny server, žiadna inštalácia).

Pri prvom použití ťa appka vyzve na zadanie vlastného **bezplatného Groq API kľúča** (získaš ho na [console.groq.com/keys](https://console.groq.com/keys)). Kľúč sa ukladá **iba lokálne v tvojom prehliadači** (localStorage) — nikam inam sa neposiela, appka nemá žiadny vlastný server.


