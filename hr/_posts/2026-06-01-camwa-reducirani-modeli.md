---
title: "Brze simulacije na domenama promjenjivog oblika"
ref: vlah-camwa
summary: "U časopisu Computers & Mathematics with Applications objavljen je rad o modelima reduciranog reda koji pomoću dubokih neuronskih mreža sami uče opis domene."
image: /assets/img/vijesti/vlah-camwa.png
image_alt: "Polje brzine strujanja u kanalu s proširenjem i eliptičnom preprekom"
image_caption: "Rješenje strujanja u kanalu s preprekom na domeni promjenjivog oblika."
---
U časopisu **Computers & Mathematics with Applications** (vol. 216, 2026., str. 282–300) objavljen je rad **Reduced order modeling of partial differential equations on parameter-dependent domains using deep neural networks** (M. Bukač, I. Mikuš, B. Muha, D. Vlah). Rad je dostupan na [doi.org/10.1016/j.camwa.2026.05.008](https://doi.org/10.1016/j.camwa.2026.05.008), a preprint na [arXiv:2407.17171](https://arxiv.org/abs/2407.17171).

Parcijalne diferencijalne jednadžbe često ovise o parametrima, pa ih treba rješavati mnogo puta. Modeli reduciranog reda uče iz unaprijed izračunatih rješenja i zatim brzo daju približno rješenje za nove parametre. Kad se mijenja i sama domena, primjerice oblik krvne žile ili položaj prepreke u kanalu, potreban je dobar opis domene, a to je teško kad je oblik složen ili mijenja topologiju.

Autori predlažu okvir koji duboke neuronske mreže koristi da iz podataka sam izvuče opis domene, bez ručno zadanih kontrolnih točaka i bez mreže konačnih elemenata, što je česta situacija u biomedicinskim primjenama. Tako se i rješenje i domena sažimaju u niskodimenzionalni latentni prikaz.

Istraživanje je djelomično financirano u okviru projekta VALOR.
