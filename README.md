
<html lang="ar">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="منصة نحن - منصة وطنية لتطوع ومشاركة الشباب تحت رعاية مؤسسة ولي العهد.">
    <title>منصة نحن - جامعة آل البيت</title>
    <link href="https://fonts.googleapis.com/css2?family=Arial:wght@400&display=swap" rel="stylesheet">
    <style>
        /* إعدادات عامة */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #3cc4cc; /* لون الخلفية الرئيسي */
            margin: 0;
            padding: 20px;
            color: #ffffcf; /* لون النص العام */
            line-height: 1.6; /* تباعد الأسطر */
            direction: rtl; /* اتجاه الكتابة من اليمين لليسار */
        }

        header {
            text-align: center;
            padding: 10px; /* تقليل مساحة الحشو في الهيدر */
            background-color: #ffffff; /* لون خلفية الهيدر */
            border-radius: 10px; /* جعل الحواف مستديرة */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        h1 {
            font-size: 1.8em; /* حجم الخط للعناوين */
            margin: 5px 0; /* تقليل المسافة حول العنوان */
            color: #40c4cc; /* لون نص العنوان */
        }

        .logo-container {
            display: flex;
            justify-content: center; /* توسيط الشعارات */
            align-items: center; /* محاذاة عمودية */
            gap: 20px; /* تباعد بين الشعارات */
            margin-bottom: 10px; /* مسافة أسفل الشعارات */
        }

        img {
            max-width: 100%; /* يسمح بعرض الصورة كاملة */
            height: auto; /* يجعل الارتفاع يتناسب تلقائياً مع العرض */
           
        }

        .logo-container img {
            width: 100px; /* تعيين عرض محدد للشعارات */
            height: auto; /* الحفاظ على نسبة العرض إلى الارتفاع */
        }

        .create-account {
            text-align: right; /* محاذاة النص إلى اليمين */
            margin-bottom: 10px; /* مسافة أسفل الزر */
        }

        .create-account a {
            background-color: #ffffff; /* لون خلفية الزر */
            color: #004d4d; /* لون النص */
            padding: 8px 12px; /* padding للزر */
            border-radius: 5px; /* حواف مستديرة */
            text-decoration: none; /* إزالة الخط السفلي */
            transition: background-color 0.3s; /* تأثير عند التمرير */
            font-weight: bold; /* جعل النص غامق */
        }

        .create-account a:hover {
            background-color: #004d4d; /* تغيير لون الخلفية عند التمرير */
            color: #ffffff; /* تغيير لون النص عند التمرير */
        }

        section {
            margin: 20px 0;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.1); /* خلفية شفافة قليلاً */
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            color: #004d4d; /* لون النص داخل العناوين */
            border-bottom: 2px solid #004d4d; /* خط سفلي تحت العناوين بلون مناسب */
            padding-bottom: 5px; /* مساحة تحت العنوان */
            font-size: 1.5em; /* حجم خط أكبر للعناوين */
        }

        p {
            color: #ffffff; /* لون النص المحايد */
            font-size: 1.1em; /* حجم خط مناسب للنصوص */
            margin: 10px 0; /* تباعد بين الفقرات */
        }

        .activity-images {
            display: flex;
            justify-content: center; /* لتوسيع الصور في الوسط */
            flex-wrap: wrap; /* للسماح بتجاوز الصور إلى السطر التالي */
            align-items: center; /* محاذاة الصور في المنتصف */
            text-align: center; /* محاذاة النص داخل القسم */
        }

        .activity-images img {
            width: 150px; /* عرض الصور */
            margin: 10px; /* مساحة بين الصور */
            border-radius: 5px; /* لجعل حواف الصور مستديرة */
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2); /* إضافة ظل خفيف للصورة */
        }

        .future-message {
            text-align: center; /* توسيط النص */
            font-size: 1.3em; /* حجم خط أكبر للرسالة */
            color: #ffffff; /* لون النص */
            margin-top: 5px; /* تقليل المسافة فوق النص */
        }

        /* تحسينات للوسائط */
        @media (max-width: 768px) {
            h1 {
                font-size: 1.5em; /* حجم الخط للعناوين في الشاشات الصغيرة */
            }

            .activity-images img {
                width: 120px; /* تقليل حجم الصور في الشاشات الصغيرة */
            }

            .logo-container img {
                width: 80px; /* حجم الشعارات في الشاشات الصغيرة */
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.2em; /* حجم الخط للعناوين في الشاشات الصغيرة جداً */
            }

            .activity-images img {
                width: 100px; /* تقليل حجم الصور أكثر في الشاشات الصغيرة جداً */
            }

            .create-account a {
                font-size: 0.9em; /* تصغير حجم الخط للزر */
            }
        }

        /* أنماط قسم السفراء */
        .ambassadors-section {
            margin-top: 20px; /* مسافة أعلى قسم السفراء */
            text-align: center; /* توسيط النص */
        }

        .ambassador {
            margin: 20px 0; /* مسافة بين السفراء */
        }

        .ambassador img {
            border-radius: 50%; /* جعل الصورة دائرية */
            width: 100px; /* عرض الصورة */
            height: 100px; /* ارتفاع الصورة */
            margin-bottom: 10px; /* مسافة أسفل الصورة */
        }

        .ambassador-name {
            font-size: 1.1em; /* حجم خط للأسماء */
            color: #ffffff; /* لون النص */
        }
    </style>
</head>

<body>

<header>
    <h1>مرحبًا بكم في بوابة سفراء نحنُ - جامعة آل البيت </h1>
    <div class="create-account">
        <a href="https://www.nahno.org/register/user/index.php" aria-label="إنشاء حساب جديد في منصة نحن">إنشاء حساب</a>
    </div>
    <div class="logo-container">
        <img src="https://assets.onecompiler.app/42wttk5ev/42wttjqj4/logo%20(2).png" alt="شعار منصة نحن">
        <img src="https://assets.onecompiler.app/42wttk5ev/42wttjqj4/22%20(3).png" alt="شعار جامعة آل البيت">
    </div>
</header>

<main>
    <section>
        <h2>تعريف عن منصة نحن</h2>
        <p>منصة "نحنُ" هي المنصة الوطنية لتطوع ومشاركة الشباب، والتي أُطلقت كأحد برامج مؤسسة ولي العهد بدعم من منظمة الأمم المتحدة للطفولة "يونيسف"، وبالتعاون مع وزارة الشباب. تهدف المنصة إلى تشجيع العمل التطوعي والمشاركة الشبابية من أجل إحداث تغيير إيجابي في المجتمعات.</p>
        <p>تعتبر "نحنُ" الأولى من نوعها في المملكة، حيث تسعى لتوحيد الجهود المبذولة في مجال العمل التطوعي. تُتيح المنصة الفرص التطوعية من مختلف مؤسسات المجتمع المدني والشركات الخاصة والقطاع العام، مما يوفر للشباب إمكانية المشاركة في الأعمال التطوعية التي تناسب اهتماماتهم.</p>
    </section>

    <section>
        <h2>دور جامعة آل البيت</h2>
        <p>تسعى جامعة آل البيت نحو أن تكون جامعة عالمية رائدة ومتميزة في مجالات التعلم والتعليم والبحث العلمي والابتكار وخدمة وتنمية المجتمع.</p>
        <p>تهدف الجامعة إلى خلق بيئة تعليمية بحثية عملية ريادية، تحفز على التفكير الإبداعي وتعزز من قيم التعاون والمشاركة والعمل الجماعي، وتضمن جودة المخرجات التعليمية.</p>
        <p>تمتاز جامعة آل البيت بمشاريعها ومبادراتها المجتمعية التي تدعم وتعزز من دور الشباب في تحقيق التنمية المستدامة.</p>
    </section>

    <section class="activity-images">
        <h2>صور الأنشطة</h2>
        <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/mafraq-1.jpg" alt="صورة نشاط 1">
        <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/252549026_1133404873858449_4639436969075829273_n.jpg" alt="صورة نشاط 2">
        <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/251979006_1133405103858426_4198342443595373620_n.jpg" alt="صورة نشاط 3">
    </section>

    <section class="future-message">
        <h2>رسالتنا إلى المستقبل</h2>
        <p>معًا نبني مستقبلًا أفضل. نحنُ نؤمن بقوة الشباب في إحداث التغيير، وسنستمر في دعم وتوفير الفرص لكل من يسعى إلى التطوع والمشاركة.</p>
    </section>

    <section class="ambassadors-section">
        <h2>سفراء جامعة آل البيت</h2>
        <div class="ambassador">
            <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/457497596_1216089772854279_8802289237022515094_n.jpg" alt="فرحان الخوالدة">
            <div class="ambassador-name">فرحان الخوالدة</div>
        </div>
        <div class="ambassador">
            <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/png-clipart-computer-icons-man-icon-logo-silhouette-thumbnail.png" alt="راشد ابو دلبوح">
            <div class="ambassador-name">راشد ابو دلبوح</div>
        </div>
        <div class="ambassador">
            <img src="https://assets.onecompiler.app/42wttk5ev/42wtwc5kj/images.png" alt="ميار هواري">
            <div class="ambassador-name">ميار هواري</div>
        </div>
    </section>
</main>
<footer>
    <p>جميع الحقوق محفوظة © 2024</p>
</footer>

</body>
</html>
