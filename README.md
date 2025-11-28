    body {
        font-family: 'Tajawal', sans-serif;
        background-color: #ffe6e6;
        color: #4a4a4a;
        overflow-x: hidden;
        padding-bottom: 50px;
        scroll-behavior: smooth; /* لتحريك الصفحة بسلاسة عند الضغط على استمرار */
    }

    .container {
        max-width: 600px;
        margin: 0 auto;
        padding: 20px;
    }

    /* تنسيق البطاقات */
    .card {
        background: white;
        border-radius: 20px;
        padding: 25px;
        margin-bottom: 20px;
        box-shadow: 0 4px 15px rgba(255, 105, 180, 0.2);
        text-align: center;
    }

    /* تنسيق الفقرات التي يتم إخفائها */
    .hidden-content {
        display: none; /* إخفاء باقي الفقرات مبدئياً */
        opacity: 0;
        transform: translateY(20px);
        transition: opacity 1s ease-in, transform 1s ease-in;
    }
    
    /* تنسيق الفقرات بعد الظهور */
    .show-content {
        display: block;
        opacity: 1;
        transform: translateY(0);
    }

    /* تنسيق الصورة */
    .main-image {
        max-width: 150px;
        height: auto;
        border-radius: 50%;
        margin-bottom: 20px;
        border: 5px solid #ff4d6d;
    }

    h1 {
        color: #ff4d6d;
        font-size: 24px;
        margin-bottom: 15px;
    }

    p {
        font-size: 18px;
        line-height: 1.6;
        margin-bottom: 10px;
    }

    /* تنسيق الشعر */
    .poem {
        font-weight: bold;
        color: #d63384;
        background-color: #fff0f5;
        padding: 15px;
        border-radius: 10px;
        border: 1px dashed #ff4d6d;
        margin: 15px 0;
    }

    /* تنسيق الأزرار (في الفقرة الأولى والأخيرة) */
    .buttons-container {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;
        margin-top: 20px;
        position: relative;
        height: 60px; 
    }

    button {
        padding: 12px 30px;
        font-size: 18px;
        border: none;
        border-radius: 50px;
        cursor: pointer;
        font-family: 'Tajawal', sans-serif;
        font-weight: bold;
        transition: transform 0.3s;
    }

    .btn-yes, .btn-continue {
        background-color: #ff4d6d;
        color: white;
        box-shadow: 0 4px 10px rgba(255, 77, 109, 0.4);
        z-index: 10;
    }

    .btn-no {
        background-color: #e0e0e0;
        color: #555;
        position: absolute; 
        left: 55%; 
    }

    /* رسالة القبول */
    #success-message {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(255, 230, 230, 0.95);
        z-index: 100;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    
    #success-message h2 {
        font-size: 30px;
        color: #ff4d6d;
    }
    
    .floating-hearts {
        color: #ff4d6d;
        font-size: 50px;
        animation: pulse 1s infinite;
    }
    @keyframes pulse {
        0% { transform: scale(1); }
        50% { transform: scale(1.2); }
        100% { transform: scale(1); }
    }

</style>
