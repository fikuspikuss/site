
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>та я не знаю шо</title>
    <div id="container">
        <div id="toggle-btn">
            <div id="moon-shape"></div>
        </div>
    </div>
</head>

<body>
    <style>
        body {
            font-family: Comic Sans MS, Comic Sans, cursive;
            margin: 20px;
            padding: 20px;
            background-color: #F1EFEF;
            color: #191717;
        }
    
        .container {
            margin: 20px;
            padding: 10px;
        }
    
        .tab-content {
            padding: 10px 20px;
            margin: 0 10px;
            cursor: pointer;
            
            border-bottom: none;
            border-radius: 5px 5px 0 0;
            
        }
    
        .image-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin: 20px;
        }
    
        .image-container img {
            max-width: 28%;
            height: auto;
            margin: 1px;
        }
        .nav-tabs {
            display: flex;
            flex-direction: row;
        }

        .nav-item {
            margin-right: 35px; /* Додано відступ між вкладками */
        }

        .nav-link.animated:hover {
            animation-name: bounce;
            animation-duration: 0.5s;
        }
            :root
{
  --main-colour:  #ffffff;
  --accent-colour: #000000;
  --moon-shape-shadow: inset 10px -9px #34306d;
  --transition: all 0.5s ease;
}

.dark-mode
{
  --main-colour:  #000000;
  --accent-colour: #ffffff;
  --moon-shape-shadow: inset 30px 30px #F7EC7D;
}

* {transition: var(--transition);}
body{ background-color: var(--main-colour); }

h1
{
  text-align: center;
  color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
h2
{
  text-align: center;
  color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
h3
{
  text-align: center;
  color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.tab-content
{
color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
#reading-tips
{
color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
#book-reviews
{
color: var(--accent-colour);
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}


#container
{
  margin: auto;
  background-color: var(--accent-colour);
  height: 119px;
  width: 280px;
  border-radius: 300px;
}

#container > div
{
  position: relative;
  top: 20px;
  left: 20px;
  background-color: var(--main-colour);
  height: 80px;
  width: 80px;
  border-radius: 300px;
  transition: transform 0.5s ease, var(--transition);
}

.dark-mode-active > div{ transform: translateX(160px);}

#container:hover{ cursor: pointer;}

#moon-shape
{
  position: absolute;
  top: 20px;
  left: 19px;
  width: 40.5px;
  height: 40.5px;
  border-radius: 50%;
  box-shadow: var(--moon-shape-shadow);
}
#scrollToTopBtn {
            position: fixed;
            bottom: 30px;
            right: 30px;
            display: none;
            background-color: rgba(61, 63, 65, 0.5);
            color: #fff;
            border: none;
            border-radius: 150%;
            padding: 15px;
            cursor: pointer;
            font-size: 30px;
        }

        #scrollToTopBtn::before {
            content: "\2191"; /* Символ стрілочки вгору */
        }

    </style>
    <script>
        const toggleBtn = document.querySelector("#container");
        const root = document.querySelector(":root");
        
        toggleBtn.addEventListener("click", e => {
            toggleBtn.classList.toggle("dark-mode-active");
            root.classList.toggle("dark-mode");
        });
        </script>
        
        <button id="scrollToTopBtn" onclick="scrollToTop()"></button>

    <!-- Підключено Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>

    <script>
        // Вивід кнопки, коли користувач прокручує сторінку вниз
        window.onscroll = function () {
            scrollFunction();
        };

        function scrollFunction() {
            var scrollToTopBtn = document.getElementById("scrollToTopBtn");

            if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
                scrollToTopBtn.style.display = "block";
            } else {
                scrollToTopBtn.style.display = "none";
            }
        }

        // Прокрутка вверх при натисканні кнопки
        function scrollToTop() {
            document.body.scrollTop = 0; // Для Safari
            document.documentElement.scrollTop = 0; // Для Chrome, Firefox, IE та Opera
        }
    </script>

    <header>
        <h1 style="font-size: 60px; font-weight: bold;">ну пакашо нема</h1>
    </header>
    

    <ul class="nav nav-tabs">
        <li class="nav-item">
            <a class="nav-link" id="my-library-tab" data-toggle="tab" href="#my-library">Моя бібліотека</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" id="book-reviews-tab" data-toggle="tab" href="#book-reviews">Рецензії на книги</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" id="reading-tips-tab" data-toggle="tab" href="#reading-tips">Рекомендації для легшого читання</a>
        </li>
        <li class="nav-item">
            <a class="nav-link active" id="my-bookshelf-tab" data-toggle="tab" href="#my-bookshelf"> some pics</a>
        </li>
    </ul>
    


    <div class="tab-content">
        


        <div class="tab-pane fade" id="my-library">
            <h2>Моя бібліотека</h2>
            <ol>
               <li><a href="https://bookclub.ua/catalog/books/pop/mesopotamiya-2" target="_blank">Месопотамія</a>, С.Жадан
                </li>
                <li><a href="https://bookchef.ua/product/yakiy-chudesniy-svit-noviy_1/" target="_blank">Який чудесний світ новий!</a>, Олдос Гакслі
                </li>
                <li><a href="https://bookchef.ua/product/volodar-muh/" target="_blank">Володар мух</a>,  Вільям Ґолдін
                </li>
                <li><a href="https://bookchef.ua/product/devyat-opovidan/" target="_blank">Дев’ять оповідань</a>, Дж. Д. Селінджер
                </li>
                <li><a href="https://bookchef.ua/product/golod1/" target="_blank">Голод</a>, Кнут Гамсун
                </li>
                <li><a href="https://bookchef.ua/product/lovets-zhiti/" target="_blank">Ловець у житі</a>, Джером Девід Селінджер
                </li>
                <li><a href="https://bookchef.ua/product/koliska-dlya-kishki-1/" target="_blank">Колиска для кішки</a>, Курт Воннеґут
                </li>
                <li><a href="https://bookchef.ua/product/mag/" target="_blank">Маг</a>,  Джон Фаулз
                </li>
                <li><a href="https://bookchef.ua/product/teatr2/" target="_blank">Театр</a>, Вільям Сомерсет Моем
                </li>
                <li><a href="https://bookchef.ua/product/boynya-nomer-p-yat-abo-hrestoviy-pohid-ditey/" target="_blank">Бойня номер п'ять, або Хрестовий похід дітей</a>, Курт Воннеґут
                </li>
                <li><a href="https://bookchef.ua/product/frankeyshteyn-abo-suchasniy-prometey/" target="_blank">Франкенштейн, або Сучасний Прометей</a>, Мері Шеллі
                </li>
                <li><a href="https://bookchef.ua/product/kolgosp-tvarin_6/" target="_blank">Колгосп тварин</a>, Джордж Орвелл
                </li>
                <li><a href="https://bookchef.ua/product/tyagar-pristrastey-lyudskih/" target="_blank">Тягар пристрастей людських</a>, Вільям Сомерсет Моем
                </li>
                <li><a href="https://bookchef.ua/product/kolektsioner_4/" target="_blank">Колекціонер</a>, Джон Фаулз
                </li>
                <li><a href="https://bookchef.ua/product/1984_orwell_1/" target="_blank">1984</a>, Джордж Орвелл
                </li>
                <li><a href="https://bookchef.ua/product/rozmalovana-vual_1/" target="_blank">Розмальована вуаль</a>, Вільям Сомерсет Моем
                </li>
                <li><a href="https://bookchef.ua/product/viktoriya-pan-golod/" target="_blank">Вікторія. Пан. Голод</a>, Кнут Гамсун
                </li>
                <li><a href="https://bookchef.ua/product/pro-mishey-i-lyudey/" target="_blank">Про мишей і людей</a>,  Джон Стейнбек
                </li>
                <li><a href="https://bookchef.ua/product/viynasvitiv/" target="_blank">Війна світів</a>, Герберт Дж. Веллс
                </li>
                <li><a href="https://bookchef.ua/product/troe-v-chovni-yak-ne-rahuvati-sobaki-/" target="_blank">Троє в човні (як не рахувати собаки!)</a>, Джером К. Джером
               // </li>
                <li><a href="https://bookchef.ua/product/portret-doriana-greya-1/" target="_blank">Портрет Доріана Ґрея</a>, Оскар Вайлд
                </li>
                <li><a href="https://bookchef.ua/product/nudota/" target="_blank">Нудота</a>, Жан-Поль Сартр
                </li>
                <li><a href="https://bookchef.ua/product/galapagos1/" target="_blank">Ґалапаґос</a>,  Курт Воннеґут
                </li>
                <li><a href="https://bookchef.ua/product/grona-gnivu/" target="_blank">Грона гніву</a>, Джон Стейнбек
                </li>
                <li><a href="https://bookchef.ua/product/z-krovi-ta-popelu-kniga-1-serii-z-krovi-ta-popelu-/" target="_blank">Кров і попіл: Із крові й попелу</a>, Дженніфер Л. Арментраут
                </li>
                <li><a href="https://bookchef.ua/product/gra-v-kota-i-mishu-kniga-1-peresliduvannya-adelini/" target="_blank">Гра в кота і мишу. Книга 1. Переслідування Аделіни</a>, Карлтон Х. Д.
                </li>
                <li><a href="https://bookchef.ua/product/tisyacha-pam-yatnih-potsilunkiv/" target="_blank">Тисяча пам’ятних поцілунків</a>, Тіллі Коул
                </li>
                <li><a href="https://bookchef.ua/product/krov-i-popil-korolivstvo-ploti-y-vognyu/" target="_blank">Кров і попіл: Королівство плоті й вогню</a>,  Дженніфер Л. Арментраут
                </li>
                <li><a href="https://bookchef.ua/product/nashi-khimichni-sertsya/" target="_blank">Наші хімічні серця</a>, Сазерленд Крістал
                </li>
                <li><a href="https://bookchef.ua/product/svoim-im-yam-mene-nazvi/" target="_blank">Називай мене своїм ім’ям</a>, Андре Асіман
                </li>
                <li><a href="https://bookchef.ua/product/sklyaniy-zamok/" target="_blank">Скляний замок</a>, Джаннетт Воллс
                </li>
                <li><a href="https://bookchef.ua/product/krov-i-popil-viyna-dvoh-korolev/" target="_blank">Кров і попіл: Війна двох королев</a>, Дженніфер Л. Арментраут
                </li>
                <li><a href="https://bookchef.ua/product/krov-i-popil-korona-z-pozolochenih-kistok-/" target="_blank">Кров і попіл: Корона з позолочених кісток</a>, Дженніфер Л. Арментраут
                </li>
                <li><a href="https://bookchef.ua/product/dim-u-voloshkovomu-mori/" target="_blank">Дім у волошковому морі</a>, Т. Дж. Клюн
                </li>
                <li><a href="https://bookchef.ua/product/klinok-korolevi-tanok-iz-tinyami/" target="_blank">Клинок королеви: Танок із тінями</a>, А. Achell
                </li>
                <li><a href="https://bookclub.ua/catalog/books/detective/i-ne-lishilos-jodnogo-2" target="_blank">І не лишилось жодного</a>, Аґата Крісті
                </li>
                <li><a href="https://bookclub.ua/catalog/books/detective/vbivstvo-u-shidnomu-ekspresi-1" target="_blank">Вбивство у «Східному експресі»</a>, Аґата Крісті
                </li>
                <li><a href="https://bookclub.ua/catalog/books/detective/pyatero-porosyat" target="_blank">П’ятеро поросят</a>,  Аґата Крісті
                </li>
                <li><a href="https://bookclub.ua/catalog/books/detective/sumniy-kiparis" target="_blank">Сумний кипарис</a>, Аґата Крісті
                </li>
                <li><a href="https://bookclub.ua/catalog/books/detective/smert-na-nili-2" target="_blank">Смерть на Нілі</a>, Аґата Крісті
                </li>
            </ol>
                <a> Ну їх взагалі 138, але самі розумієте наскільки лінь було мені їх додавати... </a> 
                
            
        </div>
    </div>
</div>

        <div class="tab-pane fade show active" id="my-bookshelf">
            <h2>smth &#128064; &#9825;</h2>
            <div class="image-container">
                <img src="сайттт/images/photo_1_2023-11-26_13-16-26.png" alt="Опис зображення">
                <img src="сайттт/images/photo_2_2023-11-26_13-16-26.png" alt="Опис зображення">
                <img src="сайттт/images/photo_3_2023-11-26_13-16-26.png" alt="Опис зображення">
               
                <img src="сайттт/images/photo_4_2023-11-26_13-16-26.png" alt="Опис зображення">
                <img src="сайттт/images/photo_5_2023-11-26_13-16-26.png" alt="Опис зображення">
                <img src="сайттт/images/photo_6_2023-11-26_12-30-46.png" alt="Опис зображення">
         
               
                <img src="сайттт/images/photo_7_2023-11-26_12-30-46.png" alt="Опис зображення">
                <img src="сайттт/images/photo_8_2023-11-26_12-30-46.png" alt="Опис зображення">
                <img src="сайттт/images/photo_9_2023-11-26_12-30-46.png" alt="Опис зображення">
    
                <img src="сайттт/images/photo_10_2023-11-26_12-30-46.png" alt="Опис зображення">
                <img src="сайттт/images/photo_11_2023-11-26_12-30-46.png" alt="Опис зображення">
                <img src="сайттт/images/photo_12_2023-11-26_12-30-46.png" alt="Опис зображення">
    
                <img src="сайттт/images/photo_13_2023-11-26_12-30-46.png" alt="Опис зображення">
                <img src="сайттт/images/photo_14_2023-11-26_12-30-46.png" alt="Опис зображення">
                
            </div>
        </div>
        <div class="tab-pane fade" id="book-reviews">
            <h2>Рецензії на книги</h2>
            <h3>Хлібне перемир'я - Сергій Жадан</h3>
            <p>У кожній дії «Хлібного перемир’я» до головних тут братів додається по новому персонажу (драматургічний прийом настільки ж старий, наскільки добре відточений). Першими прийдуть три жінки-плакальниці, у цьому колективному розумі головує тітка Шура, поруч із нею глухонімі(?) Валя й Катя; потім прибудуть сусіди-фермери: Коля і його дружина Машка, котра от-от народить; останнім буде Ренат-поштар, який приведе за собою дванадцять апостолів (закреслено) однокласників молодшого з братів, що нині вже загинули чи зникли. Як ті люди дісталися будинку, коли все горить, а мосту немає, здебільшого не ясно. У Антона забрали авто й натомість позичили надувного човна з човнярем, так і дістався берега (віва Харон; відсилка настільки очевидна, що читати її інакше як стьоб не можна). Тьотя Шура і дві її підпомагачки просто ігнорують питання, як вони тут опинилися, не здивуюся, якщо Шура вміє ходити по воді. Валя, Коля і Ренат – це все «корінне населення» місцевості, яке не виїхало чи не загинуло, але як вони вміють ходити крізь вогонь буквально, хтозна. Загартувалися? Хочеться припустити, що ті всі вже давно померли й зібралися колективно на Страшний суд. Не треба такого припускати. Патетика пізнього Метерлінка – це не про драматургію Жадана. Треба просто повірити: от ці люди всі прийшли в цей дім.
                Бо «Хлібне перемир’я» – це таки вправа на довіру.</p>

                <h3>Таємна історія - Донна Тартт</h3>
            <p>Ця книга з якоїсь причини викликає у людей невимовне захоплення. Я чула про неї звідусіль, стільки порад, стільки рекомендацій, стільки обіцянок, що вона переверне мій світ, весь мій світогляд. Спойлер: не перевернула. Книга, безперечно, цікава, але так, щоб дух захоплювало – ні, цього не сталося. Усі без винятку персонажі викликають ворожість. Серйозно, абсолютно всі – і головні, і другорядні. Сюжет будується навколо студента на ім'я Річард, від імені якого ведеться оповідання, він із небагатої сім'ї, стосунки з батьками натягнуті, він до університету їде не те щоб навчатися, він втікає. В університеті він намагається потрапити до групи студентів, які вивчають грецьку мову. До речі, я так і не зрозуміла, як влаштовано навчання в цьому університеті, але таке відчуття, що окрім грецької мови, яка була кілька разів на тиждень, більше нічого не вивчалося. Річард дивиться на маленьку групу студентів з придихом, йому дуже хочеться потрапити до їхніх лав, він заворожений. Чим? Багатством і зарозумілістю? Я не змогла розділити це почуття з Річардом, але, на жаль, слідом за Річардом я в цю групу потрапляю, починаю з усіма знайомитися. І що більше я впізнаю головних героїв, то сильніше міцніє моє бажання відрахуватися з цього наркоманського кубла. Тож мені зрозумілий від'їзд Джуліана, їхнього викладача. Спочатку мені здалося, що книга чимось схожа на «Маг» Джона Фаулза, трохи засмутилася, оскільки «Маг» мені зовсім не сподобався. Поступово у мене це почуття вивітрелося, і читання пішло легше.У процесі я раптом зрозуміла, що ця книга дуже нагадує мені серіал «Як уникнути покарання за вбивство». Є тут і схожість у сюжеті, і в характерах і ролях персонажів. Тут тобі й приналежність до особливої ​​групи студентів, обраної викладачем. І вбивство, і різні реакції головних героїв на це вбивство, і спроби приховати скоєне, і подальші злочини, які починають рости як снігова куля. Я навіть пошукала в інтернеті, чи немає зв'язку між творами – не знайшла. Я все-таки ставлю книзі хорошу оцінку, тому що мені сподобалася ідея, сюжетні ходи, але мені періодично дуже хотілося відкрити кватирку, щоб впустити трохи свіжого повітря в це прокурене, наповнене снобізмом повітря..</p>
     

        </div>
        <div class="tab-pane fade" id="reading-tips">
            <h2>Рекомендації для легшого читання</h2>
          
            <p><li style="font-size:120%;"> Обирайте цікавий матеріал: Читайте те, що вас цікавить. Це може бути художня література, наукові статті, блоги чи навіть комікси. Вибір цікавого контенту зробить читання приємнішим.</li> </p>
            <p><li style="font-size:120%;"> Встановлюйте чіткі цілі: Поставте перед собою мету, наприклад, прочитати певну кількість сторінок чи завершити главу. Це може надихнути вас на активніше читання. </li></p>
            <p><li style="font-size:120%;"> Створюйте комфортне середовище: Забезпечте собі зручне місце для читання з добрим освітленням і відповідною атмосферою. Вам буде легше зануритися в книгу, якщо у вас є комфорт. </li></p>
            <p><li style="font-size:120%;"> Визначте оптимальний час для читання: Деякі люди віддають перевагу ранковому читанню, інші - вечірньому. Знайдіть той час, коли ви найбільш зосереджені та енергійні.</li></p>
            <p><li style="font-size:120%;"> Застосовуйте метод "помідора": Розділіть час на короткі інтервали, наприклад, 25 хвилин читання, за якими слідує 5-хвилинний перерву. Це допоможе підтримувати концентрацію.</li></p>
            <p><li style="font-size:120%;"> Ведіть записи чи обговорюйте прочитане: Після читання обговорюйте матеріал з друзями чи записуйте свої враження. Це допомагає закріплювати інформацію та робить читання більш взаємодійним.</li></p>   
            <p><li style="font-size:120%;"> Експериментуйте із форматами: Спробуйте аудіокниги, електронні чи паперові книги, або комбінуйте їх. Різні формати можуть змінити ваше сприйняття матеріалу.</li></p>
        
        </div>
     
    </div>

    <footer>
        <p>&copy; 2023 паупау</p>
    </footer>
</body>

</html>
