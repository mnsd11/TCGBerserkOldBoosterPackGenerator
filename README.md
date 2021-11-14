**TCG Berserk(Old) booster pack generator**

saveimages.py - for download all .jpg images card in Berserk set for test. 
set for test - https://www.laststicker.ru/cards/berserk_equilibrium/
In https://github.com/mnsd11/TCGBerserkOldBoosterPackGenerator/Cards/ all cards sorted by values

test.py - generator boosters for 1 display (6 cards commons, seventh card - rare or ultra)
(One display have 2 ultra cards).


Known bugs:
1) In function:  
```#функция генерации частых карт  
def usually6():  
    random_index = random.randint(0, len(usually) - 1)  
    c=(usually[random_index])  
    #usually.remove(usually[random_index])#здесь оставляю remove чтобы в рамках одного бустера не повторялись частые карты, чтобы было красиво  
    buster.append(c)  
```
i commented out string for it will be work correctly for open 24 packs in display
if i just open 1 booster pack and this string is not coomented out - all 6 common cards in result is different

2) All boosters displayed in function (printed).
Need create object that will be keep all booster packs in display.

![Card example](https://www.laststicker.ru/i/cards/51/9.jpg)
