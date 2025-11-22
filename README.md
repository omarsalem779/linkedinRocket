<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🚀 LinkedIn Rocket - محسن حسابات لينكدإن</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #0077b5;
            --secondary: #00a0dc;
            --accent: #ff6b35;
            --dark: #2d3748;
            --light: #f8f9fa;
            --success: #28a745;
            --warning: #ffc107;
        }
        
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-top: 20px;
            margin-bottom: 20px;
        }
        
        /* الهيدر المحسن */
        .hero-header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 50px 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .hero-header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 1px, transparent 1px);
            background-size: 20px 20px;
            animation: float 20s linear infinite;
        }
        
        @keyframes float {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(-20px, -20px) rotate(360deg); }
        }
        
        .logo {
            font-size: 48px;
            margin-bottom: 15px;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .hero-header h1 {
            font-size: 42px;
            margin-bottom: 15px;
            font-weight: 700;
        }
        
        .hero-header p {
            font-size: 20px;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto 25px;
        }
        
        .badges {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 20px;
        }
        
        .badge {
            background: rgba(255, 255, 255, 0.2);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 14px;
            backdrop-filter: blur(10px);
        }

        /* زر الترجمة */
        .language-switcher {
            position: absolute;
            top: 20px;
            left: 20px;
        }
        
        .lang-btn {
            background: rgba(255, 255, 255, 0.2);
            border: none;
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            cursor: pointer;
            backdrop-filter: blur(10px);
            transition: all 0.3s;
        }
        
        .lang-btn:hover {
            background: rgba(255, 255, 255, 0.3);
        }
        
        /* قسم الميزات */
        .features {
            padding: 60px 30px;
            background: var(--light);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .feature-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s, box-shadow 0.3s;
            border-top: 4px solid var(--primary);
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .feature-icon {
            font-size: 40px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .feature-card h3 {
            margin-bottom: 15px;
            color: var(--dark);
        }

        /* قسم عمر سالم */
        .expert-section {
            padding: 60px 30px;
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            color: white;
            text-align: center;
        }
        
        .expert-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .expert-avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid white;
            margin: 0 auto 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
        }
        
        .expert-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        
        .stat-number {
            font-size: 32px;
            font-weight: bold;
            margin-bottom: 5px;
        }
        
        /* نموذج التحليل */
        .analyzer-section {
            padding: 50px 30px;
        }
        
        .analyzer-form {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 25px;
        }
        
        label {
            display: block;
            margin-bottom: 10px;
            font-weight: 600;
            color: var(--dark);
            font-size: 16px;
        }
        
        input, select, textarea {
            width: 100%;
            padding: 15px 20px;
            border: 2px solid #e2e8f0;
            border-radius: 12px;
            font-size: 16px;
            transition: all 0.3s;
        }
        
        input:focus, select:focus, textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(0, 119, 181, 0.1);
        }
        
        .btn {
            display: block;
            width: 100%;
            padding: 18px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0, 119, 181, 0.3);
        }
        
        .btn:active {
            transform: translateY(0);
        }

        .btn-expert {
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            max-width: 400px;
            margin: 20px auto;
        }
        
        .loading {
            display: none;
            text-align: center;
            padding: 40px;
        }
        
        .spinner {
            border: 4px solid #f3f3f3;
            border-top: 4px solid var(--primary);
            border-radius: 50%;
            width: 60px;
            height: 60px;
            animation: spin 1s linear infinite;
            margin: 0 auto 20px;
        }
        
        /* النتائج المحسنة */
        .result {
            display: none;
            padding: 40px 30px;
            background: var(--light);
            margin-top: 30px;
            border-radius: 15px;
        }
        
        .result-header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .score-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .score-circle {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: conic-gradient(var(--success) 0% 85%, #e2e8f0 85% 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        
        .score-inner {
            width: 90px;
            height: 90px;
            background: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            font-weight: bold;
            color: var(--dark);
        }
        
        .analysis-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 40px 0;
        }
        
        .analysis-card {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
        }
        
        .analysis-card h3 {
            color: var(--primary);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .tips-list {
            list-style: none;
        }
        
        .tips-list li {
            padding: 12px 0;
            border-bottom: 1px solid #f1f1f1;
            display: flex;
            align-items: flex-start;
            gap: 12px;
        }
        
        .tips-list li:last-child {
            border-bottom: none;
        }
        
        .tip-icon {
            color: var(--success);
            font-size: 18px;
            margin-top: 2px;
        }
        
        /* قسم الشهادات */
        .testimonials {
            padding: 60px 30px;
            background: linear-gradient(135deg, var(--dark) 0%, #4a5568 100%);
            color: white;
            text-align: center;
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
            line-height: 1.8;
        }
        
        .testimonial-author {
            font-weight: bold;
            color: var(--accent);
        }
        
        /* الفوتر */
        footer {
            background: var(--dark);
            color: white;
            padding: 40px 30px;
            text-align: center;
        }
        
        .footer-content {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }
        
        .social-links a {
            color: white;
            font-size: 20px;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--accent);
        }

        /* النص الإنجليزي المخفي */
        .english-text {
            display: none;
        }
        
        @media (max-width: 768px) {
            .hero-header h1 {
                font-size: 32px;
            }
            
            .hero-header p {
                font-size: 18px;
            }
            
            .features-grid,
            .analysis-grid,
            .testimonials-grid {
                grid-template-columns: 1fr;
            }
            
            .score-container {
                flex-direction: column;
            }
            
            .language-switcher {
                position: relative;
                top: 0;
                left: 0;
                text-align: center;
                margin-bottom: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- زر الترجمة -->
        <div class="language-switcher">
            <button class="lang-btn" onclick="toggleLanguage()">
                <i class="fas fa-language"></i> English
            </button>
        </div>

        <!-- الهيدر المحسن -->
        <header class="hero-header">
            <div class="logo">🚀</div>
            <h1 class="arabic-text">LinkedIn Rocket</h1>
            <h1 class="english-text" style="display: none;">LinkedIn Rocket</h1>
            
            <p class="arabic-text">حول حسابك إلى قوة مهنية لا تُقهر باستخدام الذكاء الاصطناعي</p>
            <p class="english-text" style="display: none;">Transform your profile into an unstoppable professional force with AI</p>
            
            <div class="badges">
                <div class="badge arabic-text">⭐ 5.0 تقييم</div>
                <div class="badge english-text" style="display: none;">⭐ 5.0 Rating</div>
                
                <div class="badge arabic-text">👥 2,500+ عميل</div>
                <div class="badge english-text" style="display: none;">👥 2,500+ Clients</div>
                
                <div class="badge arabic-text">🚀 نتائج فورية</div>
                <div class="badge english-text" style="display: none;">🚀 Instant Results</div>
            </div>
        </header>

        <!-- قسم الميزات -->
        <section class="features">
            <h2 class="arabic-text" style="text-align: center; margin-bottom: 20px; color: var(--dark);">لماذا تختار LinkedIn Rocket؟</h2>
            <h2 class="english-text" style="text-align: center; margin-bottom: 20px; color: var(--dark); display: none;">Why Choose LinkedIn Rocket?</h2>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🤖</div>
                    <h3 class="arabic-text">ذكاء اصطناعي متقدم</h3>
                    <h3 class="english-text" style="display: none;">Advanced AI</h3>
                    <p class="arabic-text">تحليل دقيق باستخدام أحدث تقنيات الذكاء الاصطناعي</p>
                    <p class="english-text" style="display: none;">Accurate analysis using latest AI technologies</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3 class="arabic-text">نتائج فورية</h3>
                    <h3 class="english-text" style="display: none;">Instant Results</h3>
                    <p class="arabic-text">احصل على تحليل كامل في أقل من 30 ثانية</p>
                    <p class="english-text" style="display: none;">Get complete analysis in under 30 seconds</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🎯</div>
                    <h3 class="arabic-text">نصائح مخصصة</h3>
                    <h3 class="english-text" style="display: none;">Personalized Tips</h3>
                    <p class="arabic-text">توصيات شخصية بناءً على أهدافك المهنية</p>
                    <p class="english-text" style="display: none;">Personal recommendations based on your career goals</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">📊</div>
                    <h3 class="arabic-text">تحليل شامل</h3>
                    <h3 class="english-text" style="display: none;">Comprehensive Analysis</h3>
                    <p class="arabic-text">تقييم كل جوانب حسابك بدقة واحترافية</p>
                    <p class="english-text" style="display: none;">Professional evaluation of all profile aspects</p>
                </div>
            </div>
        </section>

        <!-- قسم عمر سالم -->
        <section class="expert-section">
            <div class="expert-content">
                <div class="expert-avatar">
                    <i class="fas fa-user-tie"></i>
                </div>
                
                <h2 class="arabic-text">حلل حسابك مع عمر سالم</h2>
                <h2 class="english-text" style="display: none;">Analyze Your Profile with Omar Salem</h2>
                
                <p class="arabic-text">خبير LinkedIn معتمد مع سنوات من الخبرة في تحسين الملفات الشخصية</p>
                <p class="english-text" style="display: none;">Certified LinkedIn Expert with years of profile optimization experience</p>
                
                <div class="expert-stats">
                    <div class="stat-card">
                        <div class="stat-number">5+</div>
                        <div class="arabic-text">سنوات خبرة</div>
                        <div class="english-text" style="display: none;">Years Experience</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">2,500+</div>
                        <div class="arabic-text">عميل سعيد</div>
                        <div class="english-text" style="display: none;">Happy Clients</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">98%</div>
                        <div class="arabic-text">نسبة الرضا</div>
                        <div class="english-text" style="display: none;">Satisfaction Rate</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">4.9</div>
                        <div class="arabic-text">تقييم الخدمة</div>
                        <div class="english-text" style="display: none;">Service Rating</div>
                    </div>
                </div>
                
                <button class="btn btn-expert" onclick="analyzeWithExpert()">
                    <i class="fas fa-video"></i> 
                    <span class="arabic-text">جلسة تحليل مباشرة مع عمر</span>
                    <span class="english-text" style="display: none;">Live Analysis Session with Omar</span>
                </button>
            </div>
        </section>

        <!-- نموذج التحليل -->
        <section class="analyzer-section">
            <div class="analyzer-form">
                <h2 class="arabic-text" style="text-align: center; margin-bottom: 30px; color: var(--dark);">حلل حسابك الآن</h2>
                <h2 class="english-text" style="text-align: center; margin-bottom: 30px; color: var(--dark); display: none;">Analyze Your Profile Now</h2>
                
                <div class="form-group">
                    <label for="linkedinUrl" class="arabic-text"><i class="fas fa-link"></i> رابط حساب LinkedIn</label>
                    <label for="linkedinUrl" class="english-text" style="display: none;"><i class="fas fa-link"></i> LinkedIn Profile URL</label>
                    <input type="url" id="linkedinUrl" placeholder="https://www.linkedin.com/in/yourname" required>
                </div>
                
                <div class="form-group">
                    <label for="userGoals" class="arabic-text"><i class="fas fa-bullseye"></i> هدفك الرئيسي</label>
                    <label for="userGoals" class="english-text" style="display: none;"><i class="fas fa-bullseye"></i> Your Main Goal</label>
                    <select id="userGoals">
                        <option value="" class="arabic-text">اختر هدفك من التحليل</option>
                        <option value="" class="english-text" style="display: none;">Choose your analysis goal</option>
                        
                        <option value="job" class="arabic-text">البحث عن وظيفة جديدة</option>
                        <option value="job" class="english-text" style="display: none;">Finding a new job</option>
                        
                        <option value="clients" class="arabic-text">جذب عملاء ومشاريع</option>
                        <option value="clients" class="english-text" style="display: none;">Attracting clients and projects</option>
                        
                        <option value="networking" class="arabic-text">توسيع الشبكة المهنية</option>
                        <option value="networking" class="english-text" style="display: none;">Expanding professional network</option>
                        
                        <option value="personal-branding" class="arabic-text">بناء علامة شخصية</option>
                        <option value="personal-branding" class="english-text" style="display: none;">Building personal brand</option>
                        
                        <option value="promotion" class="arabic-text">الترقية الوظيفية</option>
                        <option value="promotion" class="english-text" style="display: none;">Career promotion</option>
                    </select>
                </div>
                
                <button class="btn" id="analyzeBtn">
                    <i class="fas fa-rocket"></i> 
                    <span class="arabic-text">ابدأ التحليل الذكي</span>
                    <span class="english-text" style="display: none;">Start Smart Analysis</span>
                </button>
                
                <div class="loading" id="loading">
                    <div class="spinner"></div>
                    <p class="arabic-text">جاري تحليل حسابك باستخدام الذكاء الاصطناعي...</p>
                    <p class="english-text" style="display: none;">Analyzing your profile with AI...</p>
                    <p class="arabic-text" style="font-size: 14px; color: #666; margin-top: 10px;">هذا قد يستغرق بضع ثوانٍ</p>
                    <p class="english-text" style="font-size: 14px; color: #666; margin-top: 10px; display: none;">This may take a few seconds</p>
                </div>
            </div>
            
            <!-- نتائج التحليل -->
            <div class="result" id="result">
                <div class="result-header">
                    <h2 class="arabic-text"><i class="fas fa-chart-bar"></i> تقرير التحليل الشامل</h2>
                    <h2 class="english-text" style="display: none;"><i class="fas fa-chart-bar"></i> Comprehensive Analysis Report</h2>
                    <p class="arabic-text">تحليل مفصل لحسابك مع نصائح عملية للتحسين</p>
                    <p class="english-text" style="display: none;">Detailed analysis of your profile with practical improvement tips</p>
                </div>
                
                <div class="score-container">
                    <div class="score-circle">
                        <div class="score-inner" id="score">8.5</div>
                    </div>
                    <div style="text-align: center;">
                        <h3 class="arabic-text" style="color: var(--dark); margin-bottom: 10px;">التقييم العام</h3>
                        <h3 class="english-text" style="color: var(--dark); margin-bottom: 10px; display: none;">Overall Rating</h3>
                        <p class="arabic-text">مستوى متقدم - يمكنك التحسين إلى 10/10</p>
                        <p class="english-text" style="display: none;">Advanced level - You can improve to 10/10</p>
                    </div>
                </div>
                
                <div class="analysis-grid">
                    <div class="analysis-card">
                        <h3 class="arabic-text"><i class="fas fa-check-circle"></i> نقاط القوة</h3>
                        <h3 class="english-text" style="display: none;"><i class="fas fa-check-circle"></i> Strengths</h3>
                        <ul class="tips-list" id="strengths">
                            <!-- سيتم ملؤها بالجافاسكريبت -->
                        </ul>
                    </div>
                    
                    <div class="analysis-card">
                        <h3 class="arabic-text"><i class="fas fa-tools"></i> مجالات التحسين</h3>
                        <h3 class="english-text" style="display: none;"><i class="fas fa-tools"></i> Improvement Areas</h3>
                        <ul class="tips-list" id="improvements">
                            <!-- سيتم ملؤها بالجافاسكريبت -->
                        </ul>
                    </div>
                    
                    <div class="analysis-card">
                        <h3 class="arabic-text"><i class="fas fa-bullseye"></i> خطة العمل</h3>
                        <h3 class="english-text" style="display: none;"><i class="fas fa-bullseye"></i> Action Plan</h3>
                        <ul class="tips-list" id="actionPlan">
                            <!-- سيتم ملؤها بالجافاسكريبت -->
                        </ul>
                    </div>
                </div>
                
                <div style="text-align: center; margin-top: 30px;">
                    <button class="btn" id="newAnalysis" style="background: var(--accent); max-width: 300px; margin: 0 auto;">
                        <i class="fas fa-redo"></i> 
                        <span class="arabic-text">تحليل حساب آخر</span>
                        <span class="english-text" style="display: none;">Analyze Another Profile</span>
                    </button>
                </div>
            </div>
        </section>

        <!-- قسم الشهادات -->
        <section class="testimonials">
            <h2 class="arabic-text">ماذا يقول عملاؤنا؟</h2>
            <h2 class="english-text" style="display: none;">What Our Clients Say?</h2>
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="testimonial-text arabic-text">
                        "بفضل LinkedIn Rocket حصلت على 3 عروض عمل في أسبوعين! التحليل كان دقيقاً والنصائح غيرت حسابي بالكامل."
                    </div>
                    <div class="testimonial-text english-text" style="display: none;">
                        "Thanks to LinkedIn Rocket, I received 3 job offers in two weeks! The analysis was accurate and the tips completely transformed my profile."
                    </div>
                    <div class="testimonial-author arabic-text">- أحمد، مدير تسويق</div>
                    <div class="testimonial-author english-text" style="display: none;">- Ahmed, Marketing Manager</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text arabic-text">
                        "كنت أعاني من جذب العملاء، بعد تطبيق النصائح زادت استفسارات العملاء بنسبة 300%. شكراً LinkedIn Rocket!"
                    </div>
                    <div class="testimonial-text english-text" style="display: none;">
                        "I was struggling to attract clients. After implementing the tips, client inquiries increased by 300%. Thank you LinkedIn Rocket!"
                    </div>
                    <div class="testimonial-author arabic-text">- سارة، مصممة مستقلة</div>
                    <div class="testimonial-author english-text" style="display: none;">- Sara, Freelance Designer</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text arabic-text">
                        "أداة رائعة! في دقائق معدودة حصلت على تحليل شامل كان سيأخذ مني أسابيع لو فعلته بنفسي."
                    </div>
                    <div class="testimonial-text english-text" style="display: none;">
                        "Amazing tool! In just minutes, I got a comprehensive analysis that would have taken me weeks to do myself."
                    </div>
                    <div class="testimonial-author arabic-text">- محمد، مطور برمجيات</div>
                    <div class="testimonial-author english-text" style="display: none;">- Mohammed, Software Developer</div>
                </div>
            </div>
        </section>

        <!-- الفوتر -->
        <footer>
            <div class="footer-content">
                <h3>LinkedIn Rocket</h3>
                <p class="arabic-text">نساعدك على تحقيق أقصى استفادة من وجودك على LinkedIn</p>
                <p class="english-text" style="display: none;">We help you maximize your LinkedIn presence</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-linkedin"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                </div>
                <p class="arabic-text">© 2023 LinkedIn Rocket. جميع الحقوق محفوظة.</p>
                <p class="english-text" style="display: none;">© 2023 LinkedIn Rocket. All rights reserved.</p>
            </div>
        </footer>
    </div>

    <script>
        // دالة الترجمة
        function toggleLanguage() {
            const arabicTexts = document.querySelectorAll('.arabic-text');
            const englishTexts = document.querySelectorAll('.english-text');
            const langBtn = document.querySelector('.lang-btn');
            
            arabicTexts.forEach(element => {
                element.style.display = element.style.display === 'none' ? '' : 'none';
            });
            
            englishTexts.forEach(element => {
                element.style.display = element.style.display === 'none' ? '' : 'none';
            });
            
            // تحديث نص زر الترجمة
            if (langBtn.innerHTML.includes('English')) {
                langBtn.innerHTML = '<i class="fas fa-language"></i> العربية';
            } else {
                langBtn.innerHTML = '<i class="fas fa-language"></i> English';
            }
        }

        // دالة جلسة عمر سالم
        function analyzeWithExpert() {
            const isEnglish = document.querySelector('.english-text').style.display === '';
            
            if (isEnglish) {
                alert("Thank you for your interest! Omar Salem will contact you within 24 hours to schedule your personalized LinkedIn analysis session.");
            } else {
                alert("شكراً لاهتمامك! عمر سالم سيتواصل معك خلال 24 ساعة لتحديد موعد جلسة تحليل LinkedIn المخصصة.");
            }
            
            // يمكنك إضافة redirect إلى نموذج حجز هنا
            // window.location.href = 'https://calendly.com/omarsalem/linkedin-analysis';
        }

        // كود التحليل الأصلي
        document.getElementById('analyzeBtn').addEventListener('click', function() {
            const linkedinUrl = document.getElementById('linkedinUrl').value;
            const userGoals = document.getElementById('userGoals').value;
            
            if (!linkedinUrl) {
                const isEnglish = document.querySelector('.english-text').style.display === '';
                alert(isEnglish ? "Please enter your LinkedIn profile URL" : "يرجى إدخال رابط حساب LinkedIn");
                return;
            }
            
            // إظهار تحميل
            document.getElementById('loading').style.display = 'block';
            document.getElementById('analyzeBtn').disabled = true;
            
            // محاكاة اتصال بالذكاء الاصطناعي
            setTimeout(() => {
                document.getElementById('loading').style.display = 'none';
                generateAIAnalysis(linkedinUrl, userGoals);
                document.getElementById('result').style.display = 'block';
                document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
            }, 3000);
        });
        
        function generateAIAnalysis(url, goals) {
            const isEnglish = document.querySelector('.english-text').style.display === '';
            
            const strengths = isEnglish ? [
                'Professional and attractive profile picture',
                'Headline clearly shows your specialization and value',
                'Strong and diverse network of connections',
                'Work experiences are excellently documented',
                'Skills section is comprehensive and well-organized'
            ] : [
                'صورة شخصية احترافية وجذابة',
                'العنوان يوضح تخصصك وقيمتك المقدمة',
                'شبكة تواصل قوية ومتنوعة',
                'الخبرات العملية موثقة بشكل ممتاز',
                'قسم المهارات شامل ومنظم'
            ];
            
            const improvements = isEnglish ? [
                'Add a cover photo that reflects your professional identity',
                'Include more digital achievements in your experiences',
                'Increase engagement with content in your field',
                'Add recommendations from colleagues and managers',
                'Improve keywords in the About section'
            ] : [
                'إضافة صورة غلاف تعبر عن هويتك المهنية',
                'تضمين المزيد من الإنجازات الرقمية في الخبرات',
                'زيادة التفاعل مع المحتوى في مجالك',
                'إضافة recommendations من زملاء ومديرين',
                'تحسين الكلمات المفتاحية في قسم About'
            ];
            
            const actionPlan = isEnglish ? [
                'Publish valuable content twice a week',
                'Engage with 5 posts daily in your field',
                'Request 3 recommendations this week',
                'Update your personal projects section',
                'Participate in specialized LinkedIn groups'
            ] : [
                'انشر محتوى قيماً مرتين أسبوعياً',
                'تفاعل مع 5 منشورات يومياً في مجالك',
                'اطلب 3 توصيات هذا الأسبوع',
                'حدث قسم المشاريع الشخصية',
                'شارك في مجموعات LinkedIn المتخصصة'
            ];
            
            // عرض النتائج
            document.getElementById('score').textContent = '8.5';
            
            const strengthsElement = document.getElementById('strengths');
            strengthsElement.innerHTML = strengths.map(strength => 
                `<li><span class="tip-icon">✅</span> ${strength}</li>`
            ).join('');
            
            const improvementsElement = document.getElementById('improvements');
            improvementsElement.innerHTML = improvements.map(improvement => 
                `<li><span class="tip-icon">🔧</span> ${improvement}</li>`
            ).join('');
            
            const actionPlanElement = document.getElementById('actionPlan');
            actionPlanElement.innerHTML = actionPlan.map(action => 
                `<li><span class="tip-icon">🎯</span> ${action}</li>`
            ).join('');
        }
        
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
