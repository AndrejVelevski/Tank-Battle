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
    
    „Rounds“ - Со оваа опција можете да наместите колку рунди ќе трае играта.
    
    „Health“ - Со оваа опција можете да наместите колку живот ќе имаат двата играчи.
    
    „Fuel“ - Со оваа опција можете да наместите колку гориво ќе имаат двата играчи.
    
    „Same weapons“ - Доколку оваа опција е селектирана, тогаш и двата играчи ќе ги имаат истите оружја
    (рандом селектирани). Доколку не е селектирана, двата играчи ќе имаат различни оружја (рандом селектирани).
    
    „Allow jumping“ - Доколку оваа опција е селектирана, тогаш за време на играта ќе биде овозможено скокање
    при што секој скок ќе одзема 20 гориво.
    
    „Visual indicators“ - Ова е опција која ви ја олеснува работата при бирање на аголот на пукање и јачината,
    со тоа што ќе имате визуелен приказ кои се границите, каде пукате и со колкава јачина.
    
    „Gravity“ - Со оваа опција ќе можете да ја наместите гравитацијата на проектилите и на играчот.
    
    „Jump speed“ - Со оваа опција ќе можете да наместите колку силно да скокаат тенковите.
    
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
во која ќе можете да направите ваш сопствен левел коj ќе можете да го играте.

Вашиот левел го дизајнирате со притискање левото копче од маусот, така што ќе „одземате“ од теренот. За „Terrain quality“
и „Debug terrain“ можете да прочитате од 4. Options.

    Во горниот лев агол можете да го напишете името на вашиот левел.

„Reset“ 

    Со притискање на ова копче, се бришат сите промени направени врз теренот, и ви се генерира нов
    терен врз кој можете повторно да работите.
    
„Save level“

    Со притискање на ова копче, левелот се серијализира со името кое што е дадено во горниот лев
    агол и екстензија .lvl, при што вие немора да се грижите каде ќе го снимите фајлот бидејќи
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
    
2. Level Select

Кога ќе кликнете на копчето „Level Select“, ви се отвара нова форма 
![Level Select](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/Level%20Select.png)
во која ќе можете да изберете кој левел ќе сакате да го играте (исто така и ваши левели). На левата страна
има листа од default левели кои ги направив во „Level Creator“ кои можете да ги изберете. На десната страна
е мал приказ (1:4 скалиран) на изгледот на левелот. Со притискање на копчето „Accept“ го избирате тој левел
за да го играте при што ви се гаси формата, а со притискање на копчето „Cancel“ ви се гаси формата, при што
ќе се избере левелот кој што предтоа бил селектиран. Кога првпат ќе се пушти апликацијата, се избира рандом
левел од сите левели кои го има во фолдерот „levels“. Доколку го нема тој фолдер, се генерира нов фолдер со
левелот со име „Blank“.

1. New Game

Кога ќе кликнете на копчето „New Game“, ви се отвара нова форма 
![New Game](https://github.com/AndrejV97/Tank-Battle/tree/master/README%20-%20SLIKI/New%20Game.png)
и играта почнува. Прв на ред е секогаш „player 1“.

Секоја рунда играчот има одредено време да го придвижи својот тенк со користење на копчињата „A“ и „D“, со што ќе се помести тенкот
лево или десно. Доколку играшот е заглавен во дупка, може да скокне со притискање на копчето „Space“. Потоа играчот може едноставно со кликање на формата (околку него), да избере со која јачина и под кој агол ќе пука. Алтернативно може да ги користи кокчињата „Q“ и „E“,
за да го наместите аголот и копчињата „W“ и „S“ за да ја наместите јачината.

За да изберете кој тип на проектил да го пукате можете да кликнете над копчето „Shoot“ при што ќе ви се отвори листа од сите оружја што
ги имате и колку имате од секој тип.

На крај за да го испукате селектираниот проектил го кликате копчето „Shoot“. После експлозијата, следен на ред е другиот играч.

________________________________________________________________________________________________________________________________________

За решението на овој проблем, најчесто се користат int, double и string податоци.

int - позицијата на терено, експлозиите и при исцртување на сите елементи (Мора да се кастира во int).

double - позиција на играчите и проектилите, гравитација, наклон. (Мора да се користи double затоа што int не е доволно прецизен. На пример default гравитацијата е 0.4. Дури и најмалата промена на ова може да доведе до видливи резултати).

string - имиња на типовите на проектили,  левелите, играчите и скоро секој текст прикажан треба да се кастира во string.

Од податочни структури искористена е само листа (од сопствени дефинирани типови) на многу места: Листа од „парчиња“ терен, листа од
проектили, листа од експлозии, листа од левели.

________________________________________________________________________________________________________________________________________

Сите функционалности се направени од мене освен следните две:

1. public bool isColliding(Blast blast)

Ова е за проверка дали се допираат круг и квадрат. Во мојот случај тоа е „парче“ терен и
експлозија. Решението го превземав од: https://stackoverflow.com/questions/401847/circle-rectangle-collision-detection-intersection

2. private double getTrajectory(Projectile p)

Ова е за се најде парабола која што зависи од гравитација, јачина и агол при истрел.
За влез се користи проектил, но само x вредноста му се зема, и по извршувањето на формулата се добива неговата y вредност. Решението го превземав од: https://en.wikipedia.org/wiki/Trajectory_of_a_projectile#Height_at_x. При што формулата е модифицирана за да може да пресмета од било која точка на теренот. Ова го направив со замена на x со делта x(растојание од координатниот почеток и x координатата на играчот).

Функцијата напишана за аголот од 90 и 270 степени е моја, бидејќи горната функција не работи за тие вредности.

________________________________________________________________________________________________________________________________________

За оваа проектна задача ќе ги објаснам (според мене) двете најважни функции:

1. private double getAngle(Player p)

Со оваа функција го наоѓаме наклонот на тенкот во зависност на каков терен стои и потоа го зимаме тој наклон и кога го цртаме тенкот го ротираме за тој наклон, со што ни се прикажува како тенкот се движи(качува или симнува) низ теренот.

За да го постигнам ова искористив равена на права од калкулус. y-y1 = k(x2-x1). Каде k е наклонот, а тој се пресметува со
(y2-y1)/(x2-x1). Позицијата x1 ја ставив да биде 8 пиксели лево од центарот на тенкот, a x2 десно 8 пиксели, а y1 i y2 ги ставив да бидат y вредноста на тенкот. Потоа местата каде што y1 и y2 се допираат со теренот и „воздухот“ ги добив така што ги ставив во for циклус(за секој y по 2 for циклуси). Ако (x1,y1) веќе се наоѓа во терен, го придвижувам y1 нагоре додека не дојдам до „воздух“, а ако (x1,y1) се наоѓа во „воздух“, го придвижувам y1 надолу се додека не дојдам до терен. Истото важи и за y2. Така ги добив двете допирни точки помеѓу теренот и „воздухот“ на растојание од 8 пиксели околу тенкот, и ја применив горно-наведената формула.

2. private void destroyTerrain(int percision, int istart, int iend, int jstart)

Со оваа функција се уништува теренот. При што се користи рекурзивно и динамичко решение(проблемите се препокриваат(АИПС)) за што побрзо да се изминат сите експлозии и секое „парче“ терен, а непотребните споредби да се избегнат.

percision - Ова е опцијата од terrain quality

istart - Ова е почетниот бројач за експлозиите, при првиот повик на функцијата ова би било 0
iend - Ова е крајниот индекс од моменталните експлозии кои се сличуваат, при првиот повик ова би било blasts.Count(вкупниот збир на експлозии).

jstart - Ова е почетниот бројач за теренот, при првиот повик ова би било 4(3+1), (бидејќи имаме вкупно 4 зида кои го заобиколуваат целиот левел, и тие се неуништливи, и затоа за нив немора споредба, а додаваме уште 1 на бројачот за да се избегне проверка на теренот од предходно т.е. првичниот терен).

Решението на ова е со два for циклуси. Првиот циклус ги изминува сите експлозии, а вториот ги изминува сите „парчиња“ терен.

Најпрво, за крај на рекурзивниот повик проверуваме дали ширината и висината на „парчето“ терен е помала или еднаква од percision. Ако ова е исполнето тогаш излегуваме од циклусот и проверуваме за наредната експлозија, а ако не е, продолжуваме со поделба на теренот.

Рекурзијата одма се започнува но овој пат istart и iend се ставаат така што се зема индексот од моменталната експлозија, и се разгледува само за таа експлозија со што новата рекурзија ќе се сведе на само 1 for циклус(бидејќи нема потреба сите останати експлозии да се разгледуваат, бидејќи подоцна за нив исто така ќе биде повикана рекурзијата). А jstart се става така што зема моменталната позиција на „парчето“ терен(ова го правиме бидејќи нема потреба повеќе да го разгледуваме целиот терен, туку теренот настанат само по разделбата која е напишана доле).

„Парчето“ терен го делиме на 4 „парчиња“ терен кои ги сместуваме во четирите агли од првичното поголемо „парче“ терен. На пример ако првичното „парче“ терен е 64x64, се прават 4 нови „парчиња“ со димензии 32x32 и се пополнуваат на негово место, а првичното „парче“ се брише.

Во мојот случај должината и висината на секое секое „парче“ се дели со 2 се додека тие не се помали или еднакви на percision (крајот на рекурзијата).

________________________________________________________________________________________________________________________________________

Проектна задача по визуелно програмирање 2017 - Андреј Велевски 152021
