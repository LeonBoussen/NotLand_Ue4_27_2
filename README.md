## NotLand
=============

# Unreal Engine Project
# Leon Boussen, Damon-Jay Jellema
===================================

## De Opdracht
### Voor het keuzedeel Preflight Check moeten we een professioneel werkprocess volgen voor het maken van een game. Het project doen we in een groepje van twee.
=====================================================================================================================

## Het Idee
### Ons idee was om een survival game te maken dat zich afspeelt op een onbewoont eiland. Jou doel is om te overleven op het eiland en een een uitweg te vinden. Ondertussen lopen er dieren op het eiland. Sommige zijn vriendelijk maar sommige zijn ook gevaarlijk.
============================================================================================================

### Geproduceerde Game Onderdelen

Leon:

* Enviroment
* Player Movement
* Player Combat
* Player and Animal Health/Death


Damon:

* Friendly Animals
* Hostile Animals
* Animal Animations

## Friendly Animals door: Damon
### De friendly animals kunnen lopen naar een willekeurige locatie, hebben stamina dus ze kunnen moe raken, ze kunnen slapen en ze kunnen wegrennen van de speler.

### Voor de Random roam gaat hij gewoon naar een willekeurige locatie binnen de aangegeven radius. En wanneer het dier damage krijgt, verdubbeld hij de loop snelheid en speelt hij een ren animatie af. Na een willekeurige afstand stopt hij met rennen en gaat hij weer rondlopen.
![](Code%20SnipBits/Roam.png)
### De stamina. wanneer het spel start gaat er elke seconde een beetje stamina af van de max stamina. Als de max stamina 0 raakt speelt hij een rust animatie en krijgt hij stamina erbij. Als hij in deze animatie zit kan hij niet bewegen. Wanneer hij genoeg heeft staat hij weer op en gaat het process opnieuw.
![](Code%20SnipBits/Stamina.png)
### Het dier heeft ook een decide action script. Dat script kijkt naar wat er gebeurt in het spel en beslist dan wat het dier gaat doen.
![](Code%20SnipBits/Decide.png)

## Hostile Animals door: Damon
### De Hostile animal werk met pawn sensing. Als de spelen in het visie van het dier komt, loopt het dier op de speler af om aan te vallen. Als het dier tegen de speler aan staat speelt hij een animatie af en doet hij damage.
![](Code%20SnipBits/Attack.png)

## Animations door: Damon
### voor elk dier zitten aparte animaties in voor lopen, rennen, rusten en aanvallen. Dit heb ik gedaan met een Animation blueprint en een Blendspace. In de blendspace staan alle animaties ingesteld dus als het dier een bepaalde snelheid haalt verandert de animatie naar de juist behorende animatie.
![](Code%20SnipBits/BS.png)
![](Code%20SnipBits/Anim.png)
