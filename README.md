# CSSTTR Demo

[NAAR DEMO](https://jamalvr.github.io/cssttr/)

Het is een website waar je zogenaamd achtergrondafbeeldingen van OSX kan bekijken/kopen. Het begint met een inlogscherm. Vervolgens kom je op een overzichtspagina met verschillende onderwerpen en een klein overzicht van beschikbare achtergronden. De gebruiker kan of naar een externe website gaan voor meer informatie, of naar het aankoopscherm in de vorm van een dialog om een achtergrond aan te schaffen.

## What I learned

Wat ik vooral heb geleerd, is dat je bizar ver met alleen CSS uit de voeten komt. Door het gebruiken van lange, omslachtige selectors wordt het duidelijk wat er allemaal mogelijk is wanneer je (bijna) geen classes gebruikt. De voorbeelden die in het boek stonden vond ik zelf leuke toepassingen om styling toe te voegen. Er stonden meerdere trucjes in die ik zelf nog nooit had gezien of gebruikt, zoals het veranderen van alleen de `Ampersand`. 

```
progress[value]::-webkit-progress-bar {
    ...
}

dialog input[type="radio"]:checked + label > svg {
    ...
}

.login + body main { 
    ...
}

main section:first-child article:hover::before {
    ...
}
```

## Components

- Login scherm
- Menu bar met dropdown
- Klikbare elementen met een modal/dialog
- Dialog met 'progress bar', aankoopproces en custom radiobuttons 
- (grote) Klikbare elementen die doorverwijzen naar de website van Vasilis

### To-do V1

1. Styles toevoegen uit hoofdstuk 6.33, 7.36, (7.38), 7.40 van CSS secrets
    - ✅ 5.25 Fancy ampersands (font-stack, cascade)
    - ✅ 6.32 De-emphasize by dimming
    - ✅ 6.33 De-emphasize by blurring
    - ✅ 7.36 Intrinsic Sizing
    - ✅ 7.40 Vertical centering
2. ✅ Texten op de cards eerst hiden, vervolgens showen op hover & focus
3. ✅ Een deel van de functionaliteiten hiden en vervolgens laten zien via een modal
4. ✅ Animaties op buttons (emoticons)
5. ✅ Background-image (eventueel parralax) op de cards toevoegen en text anders positioneren met flex-box

### To-do V2

- Modal scherm verder uitwerken
    - ✅ Progress bar 100% width
    - ✅ IMG 100% width met header er bovenop
    - ✅ Emoji's stylen
    - ✅ :hover / :focus state emoji
- ✅ Login scherm uitwerken
- ✅ Contact / Chat hiden en vervolgens laten zien
- ✅ Transitions op :hovers en :focus—8.42
- ✅ Cursor—6.29
- ✅ Extending the clickable area—6.30
- ✅ Custom checkboxes—6.31
- ✅ (Pseudo)random background—2.7
- ✅ Validatie van het formulier

### To-do V3
#### Openstaande punten

- Opschonen van de CSS.
    - Er wordt nu nog veel styling herhaald.
    - Groeperen van elementen die dezelfde styling bevatten.
- Meerdere grid elementen toevoegen zoals de Figure section.
    - Deze ook automatisch mobile friendly maken met `auto-fit`. Dit was eerder zo, maar zorgde voor bugs wanneer ik schaalde naar mobile friendly.
