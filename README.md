<div align="center">
    <h1>Motivációs levél</h1>
</div>

# Bevezetés
Mindig is jó voltam matekból. Könnyen megértettem már órán az anyagot, és mindig 5-ös voltam komolyabb otthoni tanulás nélkül.

2021 végén (7. osztály) elkezdtem magamtól programozást tanulni és a matek iránti érdeklődésem is nagyban megnőtt.

Sok programozási problémához matek szükséges, és sok matek problémában segít a programozás, így kéz a kézben tanultam őket.

# Amivel eddig foglalkoztam
Pár program, amik megírása közben sok matekot tanultam/használtam (vagy bármilyen más módon kapcsolódik a programhoz):

## Egy 2D-s játék (2022. feb.) (Python, PyGame)
- Játékmotor nélkül
- Programozás és matek tanulási célból

Trigonometria alapjait (sin, cos, arctan) megtanultam (egy olyan ellenség megírásához, ami a játékos felé lő).

<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/2d_1.png"/>
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/2d_2.png"/>

Forráskód, több kép és videók a saját [repo](https://github.com/Krist0FF-T/supermuki)-jában

## Egy 3D-s játék (2022. aug.) (C++, raylib)
- Játékmotor nélkül
- Sok trigonometriát tanultam (már volt egy alapom) (a shadereket még nem én írtam meg)

<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/3d.png"/>
<img src="https://github.com/Krist0FF-T/stuff/blob/main/minecraft_clone/0_0_6/screenshots/screenshot002.png"/>

[Forráskód](https://github.com/Krist0FF-T/stuff/tree/main/minecraft_clone)

## Feladatlap generáló (2023 jan.) (Python)
Egy képet generált egy grafikus könyvtárral, amit ki lehetett nyomtatni. (Az akkor 2.-os kistesómnak készítettem vele feladatlapokat)

<details>
    <summary>Képek</summary>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/feladatlap_1.png"/>
    <img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/feladatlap_2.png"/>
</details>

## Egyenletábrázoló (első implementáció: 2022 nov.)
### Működése
- minden pixelnél kiszámolja az egyenlet két oldalának értékét x és y behelyettesítésével és e 2 érték különbsége alapján színezi be
- világosság (0..1) = 1 / (1 + 10d) ^ 2
    - (ahol "d" a két oldal különbségének az abszolútértéke)
    - így ha d=0, akkor 1 (100%), és ahogy d nő, egyre sötétül
    - (általában ezt használtam, vagy ehhez hasonlót)
    - (több egyenlet ábrázolásánál kicsit bonyolultabb)

### Egy egyszerű példa
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/eq_sin_cos.png"/>
- piros: y = sin(x)
- kék: y = cos(x)
- négyzetrács:
    - sin(x * pi) = 0 (függőleges)
    - sin(y * pi) = 0 (vízszintes)

### Egy kicsit összetettebb példa: egy arc (részlet)
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/eq_face.png"/>

- ábrázolt egyenletek:
    - piros (szem körvonal):
        - |y - ysz| = -cos(x)
        - ha |x| < 6 (hogy a fejen kívül ne ismétlődjön)
    - kék (pupilla):
        - dsz^2 = dsz * sqrt(2)/2
    - zöld (fej és haj körvonal):
        - do = rf
        - do = rh
    - sárga (haj besatírozása):
        - sin((x - y) * 4) = 0
        - ha rh < do < rf
    - (+ egy halvány négyzetrács a feljebb említett módszerrel)

- ahol:
    - ysz = 0.6 (szemek magassága)
    - dsz = sqrt((|x| - pi)^2 + (y - ysz)^2) (távolság a jobb/bal szem középpontjától)
    - do = sqrt(x^2 + y^2) (távolság az origótól)
    - rf = 6 (fej sugara)
    - rh = rf - max(0, (|sin(pi/2 * x + 0.3)| + rf/2) * sin(alfa))
        - ahol alfa = arctan(y/x)


## Project Euler problémák megoldása
(matek x programozás problémák)

Mindenkinek ajánlom, minden nehézségben található probléma

## Mandelbrot halmaz ábrázoló
- ebből jött az ötlet az egyenletábrázoló működésére, mert nem csak azt jelöli, hogy része-e a halmaznak, hanem azt is, hogy ha nem, akkor mennyire van messze, hogy a része legyen
- sokat tanultam a komplex számokról

Ha csak fekete és fehér lenne:
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_1.png"/>

Ha világosság (0..1) = 1 - n/N:
(ahol "N" a kiszámolt iterációk száma és "n" az iteráció száma amelytől |z| > 2)
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_2.png"/>

Ráközelítve:
<img src="https://github.com/Krist0FF-T/ttk_talentum/blob/main/images/mandelbrot_3.png"/>

# Amivel a jövőben foglalkoznék
- gépi tanuláson belül főleg a mélytanulással (Python + PyTorch):
    - (alap projektekkel már elkezdtem)
    - komolyabb projektekhez nincs még meg a kellő hardverem, se a pénz rá
        - (kellene egy erős videókártya sok VRAM-mal és sok tárhely a datasetek tárolására)
    - cél: LLM-ek (pl. GPT, Llama), kép generálók (pl. DALL-E, Stable Diffusion), stb. működésének mélyebb megértése (kisebb verziók készítésével)
- még több 3D-s grafika (majd Rust + wgpu használatával) (előzőleg C++ + raylib):
    - cél: a mögötte levő matek mélyebb megértése
    - (ezúttal a shadereket is én írom majd meg)
- kriptográfia, szteganográfia:
    - cél: egy ARG készítése (mint a híres Cicada 3301)
    - (egyik barátommal mindig új módszerekkel titkosítottan kommunikálunk és ezeket össze lehetne gyűjteni)

# Befejezés
Mindennap találok valami érdekes problémát, ami leköt. Mindig van mit számolnom, min elmélkednem.

Még nem tudom, hogy pontosan mi szeretnék lenni (szoftverfejlesztő, matematikus, villamosmérnök, vagy valami más), de ez a program egy nagyszerű lehetőség, hogy legalább egyről (matematikus) dönteni tudjak.

Azt viszont már tudom, hogy a matematika fontos szerepet fog játszani az életemben, így bármilyen kimenetellel megéri.
