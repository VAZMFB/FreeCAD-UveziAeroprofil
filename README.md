# FreeCAD UveziAeroprofil Makro ([FreeCAD-ImportAirfoil](https://github.com/VAZMFB/FreeCAD-ImportAirfoil) in Serbian)

<p align="center">
  <img src="https://vazmfb.com/web/img/github/UveziAeroprofil.svg" width="150">
</p>

FreeCAD Makro za uvoz koordinata i modeliranje aeroprofila. Moguće je, korišćenjem jednostavnog dijaloga, skaliranje aeroprofila, rotacija, translacija u ravni, translacija duž razmaha, izbor ravni i glavne ose kao i pretvaranje geomerije u skicu. Omogućen je uvoz koordinata sačuvanih u najčešće korišćenim formatima.

Uvoz aeroprofila je baziran na: https://github.com/VAZMFB/Python-importAirfoil

<p align="center">
  <img src="https://vazmfb.com/web/img/github/UveziAeroprofil.png" width="800">
</p>

## Zahtevi
[FreeCAD](https://www.freecadweb.org/)<br>

Navedeni makro je testiran sa **FreeCAD 0.19**.

## Ručna instalacija
Ako se **Addon Manager** ne koristi, makro se može instalirati ručno.

* Kopirajte Python ko sa odgovarajuće stranice sa makroima.
* Otovirte meni `[Macro/Macros]`, pritisnite `[Create]`, i dodelite mu ime.
* Unesite kopirani Python kod.
* Pritisnite `[Save]` dugme i restartujte FreeCAD.
* Da bi ga pokrenuli, ponovo otvorite meni za makroe, izaberite novi makro i pritisnite `[Execute]`.

## Napomene za izlaznu ivicu

Formira se otvoreni splajn (tip BSpline). Svaki aeroprofil se obrađuje tako da se otvori profil na mestu izlazne ivice i nakon toga se profil zatvara na tom mestu pravom linijom (TEdge). Cilj ove modifikacije je da se dobije jedinstvena površ gornjake i donjake. Potrebna je samo jedna površ koja je zatvorena na mestu izlazne ivice sa drugom površi (u suporotnom može doci do presecanja površi na mestu napadne ivice što nije pogodno za dalje analize metodom konacnih elemenata).

## Način upotrebe

Pokrenite makro program i pratite uputstva.

## Licenca
Copyright (C) 2022 Miloš Petrašinović <info@vazmfb.com>
 
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as 
published by the Free Software Foundation, either version 3 of the 
License, or (at your option) any later version.
  
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
  
You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
