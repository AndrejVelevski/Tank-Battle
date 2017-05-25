# Tank-Battle

Имплементација на игра со тенкови. Играте е за 2 играчи, кои што се пукаат меѓу себе со разни видови на проектили. Идејата е превземена од играта ShellShockLive.

За овој проект, јас направив игра за 2 играчи. Секој играч има сопствен тенк кој може да го контролира. Секој тенк има живот и гориво.
Целта на играта е да го уништите непријателскиот тенк или да останете со повеќе живот на крајот од сите рунди. По крајот на сите рунди, доколку и двата тенка имаат живот поголем од 0, за победник се избира играчот со повеќе живот. Ако и двата играчи имаат еднаков живот, тогаш е нерешено. Идејата е превземена од играта ShellShockLive која може да ја видите на следниот линк: http://www.shellshocklive2.com/ или видео: https://www.youtube.com/watch?annotation_id=annotation_2866562355&feature=iv&src_vid=eGuJVAm42kg&v=Y2eKHbQ1FPQ

Најпрво кога ќе ја пиштите апликацијата ќе се најдете на главното мени кое има повеќе опции:
![Glavno Meni](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/Glavno%20Meni.png)

1. New Game
2. Level Select
3. Level Creator
4. Options
5. Read me!
6. Quit Game

Сите функционалноси ќе ги објаснам од обратен редослед бидејќи „New Game“ зависи од другите Копчиња.

6. Quit game

Кога ќе кликнете на копчето „Quit Game“, апликацијата едноставно се гаси.

5. Read me!

Кога ќе кликнете на копчето „Read me!“, ви се отвара нова форма 
![Read me!](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/Read%20me.png)
во која е објаснето на кратко како да ја играте играта и што е целта на играта.

4. Options

Кога ќе кликнете на копчето „Options“, ви се отвара нова форма
![Options](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/Options.png).
Во оваа форма се наоѓаат сите параметри кои можете да ги промените за играта различно да се однесува.

„Player 1 settings“ и „Player 2 settings“

    „Name“ - Овде можете да го напишете вашето име кое ќе ви се прикаже додека ја играте играта.
    
    „Tank Model“ - Со кликање на левото или десното копче можете да го изберете моделот на тенкот.
    
    „Tank color“ - Со кликање на ова копче ќе ви се отвори палета од бои со која ќе можете да ја
    смените бојата на тенкот.
    
„Terrain quality (1-High 32-Low)“

    Овде имате 6 опции за да изберете квалитет на терен. Под „квалитет на терен“ се мисли на колку
    „грубо“ или „мазно“ теренот ќе се деформира после експлозија на проектил.
    Ако е селектирана опцијата 1, тогаш теренот ќе изгледа „мазен“ т.е. секој пиксел ќе
    се однесува како посебен објект врз кој ќе можат да се вршат разни манипулации. И во овој случај
    ќе има повеќе објекти врз кои ќе се вршат разни манипулации и играта можно е да кочи.
    Ако е селектирана опцијата 32, тогаш теренот ќе изгледа „груб“ т.е.
    теренот ќе биде „пикселизиран“, и бидејќи овие објеќти се по-крупни т.е. зафаќаат 32x32 пиксели,
    играта побрзо ќе работи.
    
    „Terrain color“ - Со кликање на ова копче ќе можете да ја смените бојата на теренот.
    
    „Debug terrain“ - Оваа опција е само визуелна, и ќе ги прикаже границите на секое парче терен.
    
    „Destructable terrain (High)“ - Со оваа опција можете да изберете дали сакате теренот да може да
    се уништува. Доколку е селектирана оваа опција, теренот ќе се уништува и „Terrain quality“ ќе
    влијае врз тоа колку брзо ќе работи играта. Доколку оваа опција не е селектирана,
    „Terrain quality“ нема никаква улога, и играта ќе работи прилично брзо.
    
„Other settings“

    „Time(s)“ - Со оваа опција можете да наместите колку секунди ќе трае една рунда. По истекувањето
    на ова време, другиот играч е на ред.
    
    „Round“ - Со оваа опција можете да наместите колку рунди ќе трае играта.
    
    „Health“ - Со оваа опција можете да наместите колку живот ќе имаат двата играчи.
    
    „Fuel“ - Со оваа опција можете да наместите колку гориво ќе имаат двата играчи.
    
    „Same weapons“ - Доколку оваа опција е селектирана, тогаш и двата играчи ќе ги имаат истите оружја
    (рандом селектирани). Доколку не е селектирана, двата играчи ќе имаат различни оружја (рандом селектирани).
    
    „Visual indicators“ - Ова е опција која ви ја олеснува работата при бирање на аголот на пукање и јачината,
    со тоа што ќе имате визуелен приказ кои се границите, каде пукате и со колкава јачина.
    
„Accept“

    Со притискање на ова копче ги зачувувате параметрите со кои ќе играте. Притоа сите овие параметри
    се серијализираат во „settings.set“ за кога ќе ја пуштите играта наредниот пат, пак да ги имате
    истите параметри. Доколку немате „settings.set“ фајл, автоматски се креира нов со default
    вредности кога ќе ја пуштите апликацијата.
    
„Reset to defaults“

    Со притискање на ова копче ви се враќаат сите параметри како што биле првпат кога ќе ја стартувате
    апликацијата освен „Player 1 settings“ и „Player 2 settings“ (Затоа што за нив сметам дека нема потреба).
    Потоа за да ги зачувате овие параметри, треба да притиснете на копчето „Accept“
    
„Cancel“

    Со притискање на ова копче, формата „Options“ се гаси и притоа не се зајувуваат никакви промени.

3. Level Creator

Кога ќе кликнете на копчето „Level Creator“, ви се отвара нова форма 
![Level Creator](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/Level%20Creator.png)
во која ќе можете да направите ваш сопствен левел кои ќе можете да го играте.

Вашиот левел го дизајнирато со притискање левото копче од маусот, така што ќе „одземате“ од теренот. за „Terrain quality“
и „Debug terrain“ можете да прочитате од 4. Options.

    Во горниот лев агол можете да го напишете името на вашиот левел.

„Reset“ 

    Со притискање на ова копче, се бришат сите промени направени врз теренот, и ви се генерира нов
    терен врз кој можете повторно да работите.
    
„Save level“

    Со притискање на ова копче, левелот се серијализира со името кое што е дадено во горниот лев
    агол и екстензија .lvl, при што вие немора да се грижите каде ќе ги снимите фајлот бидејќи
    е направено автоматски. И потоа оваа форма се гаси, а новиот левел ќе можете подоцна да го
    изберете.

„Exit“

    Со притискање на ова копче, едноставно го гасите левел едиторот без да снимите никакви промени.
    
„Brush size“

    Со оваа опција можете да ја изберете големината на вашата експлозија со која ќе го обликувате теренот.
    
„Selection“

    „Terrain“ - Доколку оваа опција ви е селектирана, тогаш при кликање на левото копче од маусот
    ќе го обликувате теренот.
    
    „Player 1“ или „Player 2“ - Доколку оваа опција ви е селектирана, наместо да го обликувате теренот, вие ќе
    ги наместите почетните позиции на играчите.
    
„Symmetry“

    „Free“ - Доколку оваа опција е селектирана, се зема опцијата од „Selection“, и можете слободно да
    едитирате (несиметрично).
    
    „Symmetrical“ - Доколку оваа опција е селектирана, се зема опцијата од „Selection“, при што доколку ви
    е селектиран терен, се појавува уште еден „brush“ симетрично од вашата позиција, а доколку ви се 
    селектирани „Player 1“ или „Player 2“ тогаш играшите се поставуваат симетрично при кликање.
    
    „Asymmetrical“ - Доколку оваа опција е селектирана, се зема опцијата од „Selection“, при што доколку ви
    е селектиран терен, се појавува уште еден „brush“ aсиметрично од вашата позиција, а доколку ви се 
    селектирани „Player 1“ или „Player 2“ тогаш играшите се поставуваат aсиметрично при кликање.
    
„Randomize“

    При кликање на ова копче, почнува да се генерира рандом терен. Опцијата „Symmetry“, „Brush size“ и
    „Terrain quality“ влијаат врз тоа како ќе се генерира теренот. Доколку во било кој момент сакате да
    престанете со генерирање на  теренот, можете повторно да кликнете на истото копче. При генерирање
    на теренот повеќето копчиња се оневозможени додека не се престане со генерирање.
    
