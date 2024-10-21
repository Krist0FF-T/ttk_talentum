<div align="center">
    <h1>Motivációs levél</h1>
</div>

# Bevezetés
Mindig is jó voltam matekból. Könnyen megértettem már órán az anyagot, és mindig 5-ös voltam komolyabb otthoni tanulás nélkül.

2021 végén (7. osztály) elkezdtem magamtól programozást tanulni és a matek iránti érdeklődésem is nagyban megnőtt.

Sok programozási problémához matek szükséges, és sok matek problémában segít a programozás, így kéz a kézben tanultam őket.

# Amivel eddig foglalkoztam
Pár program, amik megírása közben sok matekot tanultam/használtam (vagy bármilyen más módon kapcsolódik a programhoz):

## Játékok
(játékmotor nélkül, így gyakorlatilag az egészet én írtam, csak multimédia könyvtárakat használva)

### Egy 2D-s játék
Trigonometria alapjait (sin, cos, arctan) megtanultam (egy olyan ellenség megírásával, ami a játékos felé lő).

<details>
    <summary>Képek</summary>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/2d_1.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/2d_2.png"/>
</details>

Forráskód, több kép és videók a saját [repo](https://github.com/Krist0FF-T/supermuki)-jában

### Egy 3D-s játék (MineCraft-szerű építő játék)
Sok trigonometriát tanultam (már volt egy alapom) (a shadereket még nem én írtam meg)

<details>
    <summary>Képek</summary>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/3d.png"/>
    <img src="https://github.com/Krist0FF-T/stuff/blob/main/minecraft_clone/0_0_6/screenshots/screenshot002.png"/>
    <img src="https://github.com/Krist0FF-T/stuff/blob/main/minecraft_clone/0_0_6/screenshots/screenshot003.png"/>
    <img src="https://github.com/Krist0FF-T/stuff/blob/main/minecraft_clone/0_0_6/screenshots/screenshot005.png"/>
</details>

[Forráskód](https://github.com/Krist0FF-T/stuff/tree/main/minecraft_clone)

## Eszközök
### Gyakorló lap generáló
Egy képet generált egy grafikus könytárral, amit ki lehetett nyomtatni.

<details>
    <summary>Képek</summary>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/feladatlap_1.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/feladatlap_2.png"/>
</details>

### Egyenlet ábrázoló
(pl "x^2 + y^2 = 1", "y = sin(x)", vagy akár "x^2 + (1.3y + 0.3 - sqrt(abs(x))) ^ 2 = 0")

Működése:
- minden pixelnél kiszámolja az egyenlet két oldalátnak értékét x és y behelyettesítésével és e 2 érték különbsége alapján színezi be
- világosság = 1 / (1 + 10d) ^ 2
    - (ahol "d" a két oldal különbségének az abszolútértéke)
    - így ha d=0, akkor 1 (100%), és ahogy d nő, egyre sötétül
    - (általában ezt használtam, vagy ehhez hasonlót)
    - (több egyenlet ábrázolásánál kicsit bonyolultabb)

<details>
    <summary>Képek</summary>
    piros: y = sin(x)
    kék: y = cos(x)
    négyzetrács: abs(sin(x * pi)) = 0, vagy abs(sin(y * pi)) = 0
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/eq_vis_1.png"/>
    TODO: több kép
</details>

## Egyéb
### Project Euler problémák megoldása
(matek x programozás problémák)

Mindenkinek ajánlom, minden nehézségben található probléma

### Mandelbrot halmaz ábrázoló
- ebből jött az ötlet az egyenlet ábrázoló működésére, mert nem csak azt jelöli, hogy része-e a halmaznak, hanem azt is, hogy ha nem, akkor mennyire van messze, hogy a része legyen
- sokat tanultam a komplex számokról

<details>
    <summary>Képek</summary>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_1.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_2.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_3.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_4.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_5.png"/>
</details>

# Amivel a jövőben foglalkoznék
- gépi tanuláson belül főleg a mélytanulással (Python + PyTorch):
    - (alap projektekkel már elkezdtem)
    - komolyabb projektekhez nincs még meg a kellő hardverem, se a pénz rá
        - (kellene egy erős GPU és sok tárhely a datasetek tárolására)
    - cél: LLM-ek (pl. GPT, Llama), kép generálók (pl. DALL-E, Stable Diffusion), stb. működésének mélyebb megértése (kisebb verziók készítésével)
- még több 3D-s grafika (majd Rust + wGPU használatával) (előzőleg C++ + raylib):
    - cél: a mögötte levő matek mélyebb megértése
    - (ezúttal a shadereket is én írom majd meg)
- kriptográfia, szteganográfia:
    - cél: egy ARG készítése (mint a híres Cicada 3301)
    - (egyik barátommal mindig új módszerekkel titkosítottan kommunikálunk és ezeket össze lehetne gyűjteni)

# Befejezés
Fizikából is az elsők között vagyok, mert nagyrészben matek, de komolyabban nem tanultam előre.
(Biológiából és kémiából is jó vagyok)

Mindennap találok valami érdekes problémát, ami leköt (például apukámmal minden beszélgetés során).

Még nem tudom, hogy pontosan mi szeretnék lenni (szoftverfejlesztő, matematikus, villamosmérnök, vagy valami más), de ez a program egy nagyszerű lehetőség, hogy legalább egyről (matematikus) dönteni tudjak.

Azt viszont már tudom, hogy a matematika fontos szerepet fog játszani az életemben, így bármilyen kimenetellel megéri.
