# B5-TOWN
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>القوانين</title>
    <style>
        body {
            background-color: #222;
            color: white;
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            text-align: center;
        }

        header {
            background-color: #2196F3;
            padding: 20px;
            font-size: 36px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            margin-bottom: 30px;
        }

        .buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        button {
            background-color: #2196F3;
            color: black;
            border: none;
            padding: 15px 30px;
            font-size: 20px;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        button:hover {
            transform: scale(1.1);
        }

        section {
            display: none;
            background-color: #333;
            padding: 30px;
            border-radius: 10px;
            margin-top: 20px;
            max-width: 800px;
            width: 100%;
            transition: transform 0.5s ease-in-out;
        }

        section.active {
            display: block;
            transform: scale(1.05);
        }

        h2 {
            font-size: 30px;
            margin-bottom: 20px;
        }

        ul {
            list-style-type: none;
            padding: 0;
            font-size: 20px;
        }

        ul li {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>

    <header>
        قوانين السيرفر
    </header>

    <div class="buttons">
        <button onclick="showSection('general')">قوانين العامة</button>
        <button onclick="showSection('gang')">قوانين العصابات</button>
        <button onclick="showSection('medic')">قوانين الاسعاف</button>
    </div>

    <section id="general">
        <h2>قوانين العامة</h2>
        <ul>
            <li>1 - يمنع مقاومة العسكري في حال تم استيقافك بمخالفة مرورية وحتى لو انك مطلوب او معاك ممنوعات.</li>
            <li>2 - يجب عليك تقدير موقفك وتقمص الرول بلاي.</li>
            <li>3 - RDM: القتل العشوائي بدون سبب.</li>
            <li>4 - VDM: الصدم العشوائي باستخدام المركبة كسلاح.</li>
            <li>5 - يمنع سرقة أو تدمير ممتلكات المسعفين أو العساكر.</li>
            <li>6 - يمنع قيادة سيارات السبورت في أماكن الأوف رود.</li>
            <li>7 - يمنع الاعتداء على المدنيين بدون سبب.</li>
            <li>8 - يمنع الستريم سنايب.</li>
            <li>9 - يمنع التواصل بين اللاعبين عبر الديسكورد.</li>
            <li>10 - في حال كنت مطارداً من قبل الشرطة أو شخص ما، يمنع عليك دخول المنزل.</li>
        </ul>
    </section>

    <section id="gang">
        <h2>قوانين العصابات</h2>
        <ul>
            <li>1 - سرقة ATM: عدد العساكر 4 | عدد اللاعبين 1-3</li>
            <li>2 - سرقة بقالة: عدد العساكر 4 | عدد اللاعبين 1-3</li>
            <li>3 - سرقة منزل: عدد العساكر 6 | عدد اللاعبين 2-5</li>
            <li>4 - سرقة مغسلة: عدد العساكر 6 | عدد اللاعبين 3-5</li>
            <li>5 - سرقة منزل فاخر: عدد العساكر 7 | عدد اللاعبين 3-6</li>
        </ul>
    </section>

    <section id="medic">
        <h2>قوانين الاسعاف</h2>
        <ul>
            <li>1 - يجب على المسعف أن يكون مجهزاً بكل المعدات الطبية.</li>
            <li>2 - الجدية في العمل وعدم أخذ الوظيفة على محمل كوميدي.</li>
            <li>3 - يجب عليك تسجيل الدخول إلى الخدمة + راديو الاسعاف.</li>
            <li>4 - يجب احترام الرتب الأعلى منك.</li>
            <li>5 - يجب الإبلاغ قبل التوجه لأي بلاغ وانتظار تعليمات مركز العمليات.</li>
        </ul>
    </section>

    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => section.classList.remove('active'));

            const section = document.getElementById(sectionId);
            section.classList.add('active');
        }
    </script>

</body>
</html>

شكرا لكم
