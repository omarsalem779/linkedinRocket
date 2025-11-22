<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>محلل LinkedIn الذكي - تقييم بواسطة الذكاء الاصطناعي</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0077b5 0%, #00a0dc 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }
        
        header {
            background: #0077b5;
            color: white;
            padding: 25px;
            text-align: center;
        }
        
        header h1 {
            font-size: 28px;
            margin-bottom: 10px;
        }
        
        header p {
            opacity: 0.9;
            font-size: 16px;
        }
        
        .analyzer-form {
            padding: 25px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #0077b5;
        }
        
        input, textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 16px;
            transition: all 0.3s;
        }
        
        input:focus, textarea:focus {
            outline: none;
            border-color: #0077b5;
            box-shadow: 0 0 0 2px rgba(0, 119, 181, 0.2);
        }
        
        .btn {
            display: block;
            width: 100%;
            padding: 15px;
            background: #0077b5;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .btn:hover {
            background: #005885;
        }
        
        .btn:disabled {
            background: #ccc;
            cursor: not-allowed;
        }
        
        .loading {
            display: none;
            text-align: center;
            padding: 20px;
        }
        
        .spinner {
            border: 4px solid #f3f3f3;
            border-top: 4px solid #0077b5;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            animation: spin 2s linear infinite;
            margin: 0 auto 15px;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .result {
            display: none;
            padding: 25px;
            background: #f8f9fa;
            border-radius: 10px;
            margin-top: 20px;
        }
        
        .score {
            font-size: 48px;
            font-weight: bold;
            color: #0077b5;
            margin: 20px 0;
            text-align: center;
        }
        
        .analysis-section {
            background: white;
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
            border-right: 4px solid #0077b5;
        }
        
        .analysis-section h3 {
            color: #0077b5;
            margin-bottom: 15px;
        }
        
        .improvement-tips {
            margin-top: 25px;
        }
        
        .improvement-tips ul {
            list-style-type: none;
            padding-right: 0;
        }
        
        .improvement-tips li {
            padding: 10px 0;
            border-bottom: 1px dashed #eee;
            padding-right: 15px;
            position: relative;
        }
        
        .improvement-tips li:before {
            content: "💡";
            position: absolute;
            right: -5px;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            color: white;
            margin-top: 30px;
            font-size: 14px;
        }
        
        @media (max-width: 600px) {
            .container {
                border-radius: 10px;
            }
            
            header h1 {
                font-size: 22px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🦸 محلل LinkedIn الذكي</h1>
            <p>أدخل رابط حسابك - وسيقوم الذكاء الاصطناعي بتقييمه وإعطائك نصائح مخصصة</p>
        </header>
        
        <div class="analyzer-form">
            <div class="form-group">
                <label for="linkedinUrl">رابط حساب LinkedIn</label>
                <input type="url" id="linkedinUrl" placeholder="https://www.linkedin.com/in/اسمك" required>
            </div>
            
            <div class="form-group">
                <label for="userGoals">أهدافك من الحساب (اختياري)</label>
                <select id="userGoals">
                    <option value="">اختر هدفك الرئيسي</option>
                    <option value="job">البحث عن وظيفة</option>
                    <option value="clients">جذب عملاء</option>
                    <option value="networking">التواصل المهني</option>
                    <option value="personal-branding">بناء علامة شخصية</option>
                </select>
            </div>
            
            <button class="btn" id="analyzeBtn">🔍 حلل حسابي باستخدام الذكاء الاصطناعي</button>
            
            <div class="loading" id="loading">
                <div class="spinner"></div>
                <p>جاري تحليل حسابك باستخدام DeepSeek AI...</p>
            </div>
            
            <div class="result" id="result">
                <h2>📊 تقرير التحليل الذكي</h2>
                <div class="score" id="score">8.5/10</div>
                
                <div class="analysis-section">
                    <h3>🎯 نقاط القوة</h3>
                    <div id="strengths"></div>
                </div>
                
                <div class="analysis-section">
                    <h3>⚠️ مجالات التحسين</h3>
                    <div id="improvements"></div>
                </div>
                
                <div class="analysis-section improvement-tips">
                    <h3>💡 نصائح مخصصة</h3>
                    <ul id="tipsList"></ul>
                </div>
                
                <button class="btn" id="newAnalysis" style="background: #28a745;">🔄 تحليل حساب آخر</button>
            </div>
        </div>
    </div>
    
    <footer>
        <p>مدعوم بـ DeepSeek AI - صمم لمساعدة المحترفين على تطوير وجودهم الرقمي</p>
        <p>© 2023 - جميع الحقوق محفوظة</p>
    </footer>

    <script>
        // محاكاة اتصال بالذكاء الاصطناعي
        document.getElementById('analyzeBtn').addEventListener('click', function() {
            const linkedinUrl = document.getElementById('linkedinUrl').value;
            const userGoals = document.getElementById('userGoals').value;
            
            if (!linkedinUrl) {
                alert('يرجى إدخال رابط حساب LinkedIn');
                return;
            }
            
            // إظهار تحميل
            document.getElementById('loading').style.display = 'block';
            document.getElementById('analyzeBtn').disabled = true;
            
            // محاكاة اتصال بالذكاء الاصطناعي (3 ثواني)
            setTimeout(() => {
                // إخفاء التحميل
                document.getElementById('loading').style.display = 'none';
                
                // توليد تحليل عشوائي (في الواقع الفعلي سيكون من DeepSeek API)
                generateAIAnalysis(linkedinUrl, userGoals);
                
                // إظهار النتيجة
                document.getElementById('result').style.display = 'block';
                
                // التمرير إلى النتيجة
                document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
            }, 3000);
        });
        
        function generateAIAnalysis(url, goals) {
            // في الواقع الفعلي، هنا سيتم الاتصال بـ DeepSeek API
            // لكن الآن سنعمل محاكاة للتحليل
            
            const strengthsList = [
                '📸 صورتك الشخصية ممتازة واحترافية',
                '✍️ قسم "About" مكتوب بطريقة مقنعة',
                '🔗 لديك شبكة تواصل جيدة',
                '💼 الخبرات العملية موثقة بشكل ممتاز',
                '🏆 الإنجازات مدعومة بأرقام ونتائج'
            ];
            
            const improvementsList = [
                '🌅 يمكنك إضافة صورة غلاف تعبر عن هويتك المهنية',
                '🔍 قسم المهارات يحتاج إلى مزيد من التفصيل',
                '📈 يمكنك زيادة التفاعل بالنشر المنتظم',
                '🤝 حاول الحصول على المزيد من التوصيات',
                '🎯 ركز أكثر على الكلمات المفتاحية في تخصصك'
            ];
            
            const tipsList = [
                'انشر محتوى قيماً مرتين أسبوعياً على الأقل',
                'شارك في التعليقات على منشورات الآخرين في مجالك',
                'أضف مشاريع شخصية إلى قسم الخبرات',
                'استخدم الكلمات المفتاحية المناسبة في العنوان',
                'اطلبه توصيات من زملاء ومديرين سابقين'
            ];
            
            // إضافة نصائح حسب الهدف
            if (goals === 'job') {
                tipsList.push('ركز على مهارات التوظيف المطلوبة في سوق العمل');
                tipsList.push('أضف كلمات مفتاحية تبحث عنها شركات التوظيف');
            } else if (goals === 'clients') {
                tipsList.push('أنشئ محتوى يظهر خبرتك ويجذب العملاء المحتملين');
                tipsList.push('شارك case studies لمشاريع ناجحة');
            }
            
            // عرض النتائج
            document.getElementById('score').textContent = '8.5/10';
            
            const strengthsElement = document.getElementById('strengths');
            strengthsElement.innerHTML = strengthsList.map(strength => 
                `<p>✅ ${strength}</p>`
            ).join('');
            
            const improvementsElement = document.getElementById('improvements');
            improvementsElement.innerHTML = improvementsList.map(improvement => 
                `<p>🔧 ${improvement}</p>`
            ).join('');
            
            const tipsListElement = document.getElementById('tipsList');
            tipsListElement.innerHTML = tipsList.map(tip => 
                `<li>${tip}</li>`
            ).join('');
        }
        
        // زر تحليل جديد
        document.getElementById('newAnalysis').addEventListener('click', function() {
            document.getElementById('linkedinUrl').value = '';
            document.getElementById('userGoals').value = '';
            document.getElementById('result').style.display = 'none';
            document.getElementById('analyzeBtn').disabled = false;
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });
    </script>
</body>
</html>
