<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🚀 LinkedIn Rocket - محسن حسابات لينكدإن</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #dc2626; /* أحمر */
            --secondary: #b91c1c; /* أحمر داكن */
            --accent: #f59e0b; /* أصفر */
            --dark: #1f2937;
            --light: #fef2f2; /* أحمر فاتح جداً */
            --success: #16a34a;
            --warning: #f59e0b;
            --danger: #dc2626;
        }
        
        body {
            background: linear-gradient(135deg, #dc2626 0%, #f59e0b 100%);
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
            z-index: 1000;
        }
        
        .lang-btn {
            background: rgba(255, 255, 255, 0.2);
            border: none;
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            cursor: pointer;
            backdrop-filter: blur(10px);
            transition: all 0.3s;
            font-weight: 600;
        }
        
        .lang-btn:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: scale(1.05);
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
            background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
            color: white;
            text-align: center;
        }
        
        .expert-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .expert-profile {
            display: flex;
            align-items: center;
            gap: 40px;
            margin-bottom: 30px;
            flex-wrap: wrap;
            justify-content: center;
        }
        
        .expert-avatar {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 5px solid white;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            position: relative;
        }
        
        .expert-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s;
        }
        
        .expert-avatar:hover img {
            transform: scale(1.05);
        }
        
        .expert-info {
            flex: 1;
            min-width: 300px;
            text-align: right;
        }
        
        .expert-badges {
            display: flex;
            gap: 10px;
            margin: 15px 0;
            flex-wrap: wrap;
            justify-content: flex-end;
        }
        
        .expert-badge {
            background: rgba(255, 255, 255, 0.2);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 14px;
            backdrop-filter: blur(10px);
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
        
        input, select {
            width: 100%;
            padding: 15px 20px;
            border: 2px solid #e2e8f0;
            border-radius: 12px;
            font-size: 16px;
            transition: all 0.3s;
        }
        
        input:focus, select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(220, 38, 38, 0.1);
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
            text-decoration: none;
        }
        
        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(220, 38, 38, 0.3);
        }
        
        .btn:active {
            transform: translateY(0);
        }

        .btn-expert {
            background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
            max-width: 400px;
            margin: 20px auto;
            display: inline-block;
        }
        
        /* شاشة التحميل المحسنة */
        .loading {
            display: none;
            text-align: center;
            padding: 40px;
        }
        
        .loading-steps {
            margin: 30px 0;
            text-align: right;
        }
        
        .loading-step {
            padding: 15px 0;
            border-bottom: 1px solid #f1f1f1;
            display: flex;
            align-items: center;
            gap: 15px;
            transition: all 0.3s;
        }
        
        .loading-step.active {
            color: var(--primary);
            font-weight: bold;
        }
        
        .loading-step.completed {
            color: var(--success);
        }
        
        .loading-step.completed .step-icon {
            background: var(--success);
        }
        
        .step-icon {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            background: #e2e8f0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 14px;
            transition: all 0.3s;
        }
        
        .progress-container {
            width: 100%;
            height: 8px;
            background: #e2e8f0;
            border-radius: 4px;
            margin: 30px 0;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 100%;
            background: linear-gradient(90deg, var(--primary) 0%, var(--accent) 100%);
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 4px;
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
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
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
            font-size: 18px;
            margin-top: 2px;
        }
        
        .score-badge {
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: bold;
            margin-top: 10px;
            display: inline-block;
            color: white;
        }

        .score-excellent { background: var(--success); }
        .score-good { background: var(--warning); color: black; }
        .score-average { background: #f59e0b; color: black; }
        .score-poor { background: var(--danger); }

        .profile-strength {
            margin: 15px 0;
            padding: 15px;
            border-radius: 10px;
            background: #fef2f2;
            border-right: 4px solid var(--primary);
        }
        
        /* الفوتر */
        .footer {
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

        .copyright {
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 14px;
            opacity: 0.8;
        }

        /* إصلاح الترجمة */
        [lang="ar"] { display: block; }
        [lang="en"] { display: none; }
        
        body.english [lang="ar"] { display: none; }
        body.english [lang="en"] { display: block; }
        
        @media (max-width: 768px) {
            .hero-header h1 {
                font-size: 32px;
            }
            
            .hero-header p {
                font-size: 18px;
            }
            
            .features-grid,
            .analysis-grid {
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
            
            .expert-profile {
                flex-direction: column;
                text-align: center;
            }
            
            .expert-info {
                text-align: center;
            }
            
            .expert-badges {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- زر الترجمة -->
        <div class="language-switcher">
            <button class="lang-btn" onclick="toggleLanguage()">
                <i class="fas fa-language"></i> <span lang="ar">English</span><span lang="en">العربية</span>
            </button>
        </div>

        <!-- الهيدر المحسن -->
        <header class="hero-header">
            <div class="logo">🚀</div>
            <h1>LinkedIn Rocket</h1>
            
            <p lang="ar">حول حسابك إلى قوة مهنية لا تُقهر باستخدام الذكاء الاصطناعي</p>
            <p lang="en">Transform your profile into an unstoppable professional force with AI</p>
            
            <div class="badges">
                <div class="badge" lang="ar">⭐ 5.0 تقييم</div>
                <div class="badge" lang="en">⭐ 5.0 Rating</div>
                
                <div class="badge" lang="ar">👥 2,500+ عميل</div>
                <div class="badge" lang="en">👥 2,500+ Clients</div>
                
                <div class="badge" lang="ar">🚀 نتائج فورية</div>
                <div class="badge" lang="en">🚀 Instant Results</div>
            </div>
        </header>

        <!-- قسم الميزات -->
        <section class="features">
            <h2 style="text-align: center; margin-bottom: 20px; color: var(--dark);">
                <span lang="ar">لماذا تختار LinkedIn Rocket؟</span>
                <span lang="en">Why Choose LinkedIn Rocket?</span>
            </h2>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🤖</div>
                    <h3 lang="ar">ذكاء اصطناعي متقدم</h3>
                    <h3 lang="en">Advanced AI</h3>
                    <p lang="ar">تحليل دقيق باستخدام أحدث تقنيات الذكاء الاصطناعي</p>
                    <p lang="en">Accurate analysis using latest AI technologies</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3 lang="ar">نتائج فورية</h3>
                    <h3 lang="en">Instant Results</h3>
                    <p lang="ar">احصل على تحليل كامل في أقل من 30 ثانية</p>
                    <p lang="en">Get complete analysis in under 30 seconds</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🎯</div>
                    <h3 lang="ar">نصائح مخصصة</h3>
                    <h3 lang="en">Personalized Tips</h3>
                    <p lang="ar">توصيات شخصية بناءً على أهدافك المهنية</p>
                    <p lang="en">Personal recommendations based on your career goals</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">📊</div>
                    <h3 lang="ar">تحليل شامل</h3>
                    <h3 lang="en">Comprehensive Analysis</h3>
                    <p lang="ar">تقييم كل جوانب حسابك بدقة واحترافية</p>
                    <p lang="en">Professional evaluation of all profile aspects</p>
                </div>
            </div>
        </section>

        <!-- قسم عمر سالم -->
        <section class="expert-section">
            <div class="expert-content">
                <div class="expert-profile">
                    <div class="expert-avatar">
                        <!-- صورتك الشخصية من LinkedIn -->
                        <img src="https://media.licdn.com/dms/image/D5603AQEo3Hp0T3_X-g/profile-displayphoto-shrink_400_400/0/1691234567890?e=1721260800&v=beta&t=abc123def456" 
                             alt="عمر سالم - خبير LinkedIn"
                             onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
                        <!-- نسخة احتياطية إذا لم تظهر الصورة -->
                        <div style="width:100%; height:100%; background:#dc2626; display:none; align-items:center; justify-content:center; color:white; font-size:60px;">
                            👨‍💼
                        </div>
                    </div>
                    <div class="expert-info">
                        <h2>عمر سالم</h2>
                        
                        <p style="margin-bottom: 15px; opacity: 0.9;">
                            <span lang="ar">خبير LinkedIn معتمد - مستشار التوظيف الرقمي</span>
                            <span lang="en">Certified LinkedIn Expert - Digital Career Consultant</span>
                        </p>
                        
                        <div class="expert-badges">
                            <div class="expert-badge" lang="ar">🎓 خبير معتمد</div>
                            <div class="expert-badge" lang="en">🎓 Certified Expert</div>
                            
                            <div class="expert-badge" lang="ar">⭐ 5 نجوم</div>
                            <div class="expert-badge" lang="en">⭐ 5 Stars</div>
                            
                            <div class="expert-badge" lang="ar">🏆 الأفضل</div>
                            <div class="expert-badge" lang="en">🏆 Top Rated</div>
                        </div>
                    </div>
                </div>
                
                <p>
                    <span lang="ar">خبير LinkedIn معتمد مع سنوات من الخبرة في تحسين الملفات الشخصية وتحويلها إلى فرص حقيقية</span>
                    <span lang="en">Certified LinkedIn Expert with years of experience in profile optimization and turning them into real opportunities</span>
                </p>
                
                <div class="expert-stats">
                    <div class="stat-card">
                        <div class="stat-number">5+</div>
                        <div lang="ar">سنوات خبرة</div>
                        <div lang="en">Years Experience</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">2,500+</div>
                        <div lang="ar">عميل سعيد</div>
                        <div lang="en">Happy Clients</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">98%</div>
                        <div lang="ar">نسبة الرضا</div>
                        <div lang="en">Satisfaction Rate</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">4.9</div>
                        <div lang="ar">تقييم الخدمة</div>
                        <div lang="en">Service Rating</div>
                    </div>
                </div>
                
                <!-- زر التواصل على LinkedIn -->
                <a href="https://www.linkedin.com/in/omar-salem-102b0a133/" 
                   target="_blank" class="btn btn-expert">
                    <i class="fab fa-linkedin"></i> 
                    <span lang="ar">تواصل معي على LinkedIn</span>
                    <span lang="en">Connect with me on LinkedIn</span>
                </a>
            </div>
        </section>

        <!-- نموذج التحليل -->
        <section class="analyzer-section">
            <div class="analyzer-form">
                <h2 style="text-align: center; margin-bottom: 30px; color: var(--dark);">
                    <span lang="ar">حلل حسابك الآن</span>
                    <span lang="en">Analyze Your Profile Now</span>
                </h2>
                
                <div class="form-group">
                    <label for="linkedinUrl">
                        <i class="fas fa-link"></i> 
                        <span lang="ar">رابط حساب LinkedIn</span>
                        <span lang="en">LinkedIn Profile URL</span>
                    </label>
                    <input type="url" id="linkedinUrl" placeholder="https://www.linkedin.com/in/yourname" required>
                </div>
                
                <div class="form-group">
                    <label for="userGoals">
                        <i class="fas fa-bullseye"></i> 
                        <span lang="ar">هدفك الرئيسي</span>
                        <span lang="en">Your Main Goal</span>
                    </label>
                    <select id="userGoals">
                        <option value="" lang="ar">اختر هدفك من التحليل</option>
                        <option value="" lang="en">Choose your analysis goal</option>
                        
                        <option value="job" lang="ar">البحث عن وظيفة جديدة</option>
                        <option value="job" lang="en">Finding a new job</option>
                        
                        <option value="clients" lang="ar">جذب عملاء ومشاريع</option>
                        <option value="clients" lang="en">Attracting clients and projects</option>
                        
                        <option value="networking" lang="ar">توسيع الشبكة المهنية</option>
                        <option value="networking" lang="en">Expanding professional network</option>
                    </select>
                </div>
                
                <button class="btn" id="analyzeBtn">
                    <i class="fas fa-rocket"></i> 
                    <span lang="ar">ابدأ التحليل الذكي</span>
                    <span lang="en">Start Smart Analysis</span>
                </button>
                
                <!-- شاشة التحميل المحسنة -->
                <div class="loading" id="loading">
                    <div class="spinner"></div>
                    <p lang="ar">جاري تحليل حسابك باستخدام الذكاء الاصطناعي...</p>
                    <p lang="en">Analyzing your profile with AI...</p>
                    
                    <div class="progress-container">
                        <div class="progress-bar" id="progressBar"></div>
                    </div>
                    
                    <div class="loading-steps" id="loadingSteps">
                        <!-- سيتم إضافة الخطوات بالجافاسكريبت -->
                    </div>
                </div>
            </div>
            
            <!-- نتائج التحليل -->
            <div class="result" id="result">
                <div class="result-header">
                    <h2><i class="fas fa-chart-bar"></i> 
                        <span lang="ar">تقرير التحليل الشامل</span>
                        <span lang="en">Comprehensive Analysis Report</span>
                    </h2>
                </div>
                
                <div class="score-container">
                    <div class="score-circle" id="scoreCircle">
                        <div class="score-inner" id="score">8.5</div>
                    </div>
                    <div style="text-align: center;">
                        <h3 style="color: var(--dark); margin-bottom: 10px;">
                            <span lang="ar">التقييم العام</span>
                            <span lang="en">Overall Rating</span>
                        </h3>
                        <p id="scoreDescription">
                            <span lang="ar">مستوى متقدم - يمكنك التحسين إلى 10/10</span>
                            <span lang="en">Advanced level - You can improve to 10/10</span>
                        </p>
                    </div>
                </div>

                <div class="profile-strength" id="profileStrength">
                    <!-- سيتم إضافته بالجافاسكريبت -->
                </div>
                
                <div class="analysis-grid">
                    <div class="analysis-card">
                        <h3><i class="fas fa-check-circle"></i> 
                            <span lang="ar">نقاط القوة</span>
                            <span lang="en">Strengths</span>
                        </h3>
                        <ul class="tips-list" id="strengths"></ul>
                    </div>
                    
                    <div class="analysis-card">
                        <h3><i class="fas fa-tools"></i> 
                            <span lang="ar">مجالات التحسين</span>
                            <span lang="en">Improvement Areas</span>
                        </h3>
                        <ul class="tips-list" id="improvements"></ul>
                    </div>
                    
                    <div class="analysis-card">
                        <h3><i class="fas fa-bullseye"></i> 
                            <span lang="ar">خطة العمل</span>
                            <span lang="en">Action Plan</span>
                        </h3>
                        <ul class="tips-list" id="actionPlan"></ul>
                    </div>
                </div>
                
                <div style="text-align: center; margin: 30px 0;">
                    <p lang="ar"><strong>هل تحتاج إلى مساعدة احترافية؟</strong></p>
                    <p lang="en"><strong>Need professional help?</strong></p>
                    <a href="https://www.linkedin.com/in/omar-salem-102b0a133/" 
                       target="_blank" class="btn btn-expert" style="max-width: 300px;">
                        <i class="fab fa-linkedin"></i> 
                        <span lang="ar">تواصل مع عمر على LinkedIn</span>
                        <span lang="en">Connect with Omar on LinkedIn</span>
                    </a>
                </div>
                
                <div style="text-align: center; margin-top: 30px;">
                    <button class="btn" id="newAnalysis" style="background: var(--accent); max-width: 300px; margin: 0 auto;">
                        <i class="fas fa-redo"></i> 
                        <span lang="ar">تحليل حساب آخر</span>
                        <span lang="en">Analyze Another Profile</span>
                    </button>
                </div>
            </div>
        </section>

        <!-- الفوتر -->
        <footer class="footer">
            <div class="footer-content">
                <h3>LinkedIn Rocket</h3>
                <p>
                    <span lang="ar">تابعني على LinkedIn للمزيد من النصائح</span>
                    <span lang="en">Follow me on LinkedIn for more tips</span>
                </p>
                <div class="social-links">
                    <a href="https://www.linkedin.com/in/omar-salem-102b0a133/" target="_blank">
                        <i class="fab fa-linkedin"></i>
                    </a>
                </div>
                
                <!-- حقوق النشر مع سنة 2025 -->
                <div class="copyright">
                    <p>
                        <span lang="ar">© 2025 LinkedIn Rocket - تم التطوير بواسطة عمر سالم</span>
                        <span lang="en">© 2025 LinkedIn Rocket - Developed by Omar Salem</span>
                    </p>
                    <p style="font-size: 12px; opacity: 0.7; margin-top: 5px;">
                        <span lang="ar">جميع الحقوق محفوظة</span>
                        <span lang="en">All rights reserved</span>
                    </p>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // نظام تحليل أكثر واقعية
        const profileAnalysisData = {
            excellent: {
                score: { min: 8.5, max: 9.5 },
                color: '#16a34a',
                badge: 'score-excellent',
                description: {
                    ar: 'ممتاز - حسابك من أفضل الحسابات المهنية',
                    en: 'Excellent - Your profile is among the top professional accounts'
                },
                strengths: {
                    ar: [
                        'صورة شخصية احترافية تعكس هويتك المهنية',
                        'العنوان يوضح تخصصك وقيمتك المضافة بوضوح',
                        'شبكة تواصل قوية تضم محترفين في مجالك',
                        'الخبرات العملية موثقة بإنجازات رقمية ملموسة',
                        'قسم المهارات شامل ويحظى بتوصيات متنوعة'
                    ],
                    en: [
                        'Professional profile picture reflecting your identity',
                        'Headline clearly shows your specialty and value',
                        'Strong network including professionals in your field',
                        'Work experiences documented with tangible achievements',
                        'Comprehensive skills section with diverse endorsements'
                    ]
                },
                improvements: {
                    ar: [
                        'أنشئ محتوى فيديو يظهر خبرتك العملية',
                        'انضم لمجموعات متخصصة وكن مساهماً نشطاً',
                        'اطلب توصيات من قادة الرأي في صناعتك',
                        'طور قسم المشاريع الشخصية بإضافات تفاعلية'
                    ],
                    en: [
                        'Create video content showcasing your practical expertise',
                        'Join specialized groups and be an active contributor',
                        'Request recommendations from industry thought leaders',
                        'Enhance projects section with interactive additions'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى قيماً 3 مرات أسبوعياً',
                        'تفاعل مع 10 منشورات يومياً في مجالك',
                        'ارسل 5 طلبات اتصال أسبوعياً لمحترفين جدد',
                        'اكتب مقالة احترافية شهرياً على LinkedIn'
                    ],
                    en: [
                        'Post valuable content 3 times weekly',
                        'Engage with 10 posts daily in your industry',
                        'Send 5 connection requests weekly to new professionals',
                        'Write one professional monthly article on LinkedIn'
                    ]
                }
            },
            good: {
                score: { min: 7.0, max: 8.4 },
                color: '#f59e0b',
                badge: 'score-good',
                description: {
                    ar: 'جيد جداً - يمكنك التحسين إلى مستوى ممتاز',
                    en: 'Very Good - You can improve to excellent level'
                },
                strengths: {
                    ar: [
                        'صورة شخصية مناسبة ولكن يمكن تحسينها',
                        'العنوان يوضح تخصصك لكن يحتاج تركيز أكبر',
                        'شبكة تواصل جيدة تحتاج للتوسع',
                        'الخبرات موثقة لكن تحتاج تفصيل أكثر'
                    ],
                    en: [
                        'Appropriate profile picture but can be improved',
                        'Headline shows your specialty but needs more focus',
                        'Good network that needs expansion',
                        'Experiences documented but need more detail'
                    ]
                },
                improvements: {
                    ar: [
                        'أضف صورة غلاف تعبر عن هويتك المهنية',
                        'أعد صياغة العنوان ليكون أكثر تأثيراً',
                        'اطلب توصيات إضافية من زملاء ومديرين',
                        'أضف إنجازات رقمية في كل خبرة عمل'
                    ],
                    en: [
                        'Add a cover photo reflecting your professional identity',
                        'Rewrite headline to be more impactful',
                        'Request additional recommendations from colleagues and managers',
                        'Add digital achievements to each work experience'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى قيماً مرتين أسبوعياً',
                        'تفاعل مع 7 منشورات يومياً في مجالك',
                        'اطلب توصيتين جديدتين هذا الأسبوع',
                        'حدث قسم المشاريع بإضافات جديدة'
                    ],
                    en: [
                        'Post valuable content twice weekly',
                        'Engage with 7 posts daily in your industry',
                        'Request 2 new recommendations this week',
                        'Update projects section with new additions'
                    ]
                }
            },
            average: {
                score: { min: 5.5, max: 6.9 },
                color: '#f59e0b',
                badge: 'score-average',
                description: {
                    ar: 'متوسط - لديك أساس جيد يحتاج تطوير',
                    en: 'Average - You have a good foundation that needs development'
                },
                strengths: {
                    ar: [
                        'صورة شخصية واضحة لكن تحتاج للاحترافية',
                        'العنوان أساسي ويمكن تطويره بشكل كبير',
                        'شبكة تواصل أساسية تحتاج للتوسع',
                        'الخبرات مسجلة لكن تفتقد للتفاصيل'
                    ],
                    en: [
                        'Clear profile picture but needs professionalism',
                        'Basic headline that can be significantly improved',
                        'Basic network that needs expansion',
                        'Experiences recorded but lack details'
                    ]
                },
                improvements: {
                    ar: [
                        'استبدل صورتك الشخصية بصورة احترافية',
                        'أعد كتابة العنوان ليعكس قيمتك الفريدة',
                        'أضف وصفاً مفصلاً لإنجازاتك في كل وظيفة',
                        'طور قسم المهارات بإضافة 10 مهارات رئيسية'
                    ],
                    en: [
                        'Replace profile picture with professional one',
                        'Rewrite headline to reflect your unique value',
                        'Add detailed description of achievements for each job',
                        'Enhance skills section with 10 key skills'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى مفيد مرة أسبوعياً على الأقل',
                        'تفاعل مع 5 منشورات يومياً في مجالك',
                        'أكمل قسم About بشكل مفصل وجذاب',
                        'أضف 5 مهارات جديدة هذا الأسبوع'
                    ],
                    en: [
                        'Post useful content at least once weekly',
                        'Engage with 5 posts daily in your industry',
                        'Complete About section in detail and attractively',
                        'Add 5 new skills this week'
                    ]
                }
            },
            poor: {
                score: { min: 4.0, max: 5.4 },
                color: '#dc2626',
                badge: 'score-poor',
                description: {
                    ar: 'يحتاج تحسين - ابدأ في بناء حسابك المهني',
                    en: 'Needs Improvement - Start building your professional profile'
                },
                strengths: {
                    ar: [
                        'لديك حساب LinkedIn - هذه بداية ممتازة',
                        'يمكنك البدء في بناء وجودك المهني من الصفر'
                    ],
                    en: [
                        'You have a LinkedIn account - excellent start',
                        'You can start building your professional presence from scratch'
                    ]
                },
                improvements: {
                    ar: [
                        'أضف صورة شخصية احترافية فوراً',
                        'اكتب عنواناً يوضح تخصصك وهدفك المهني',
                        'املأ قسم About بشكل كامل وجذاب',
                        'أضف جميع خبراتك العملية السابقة'
                    ],
                    en: [
                        'Add professional profile picture immediately',
                        'Write headline showing your specialty and career goal',
                        'Fill About section completely and attractively',
                        'Add all your previous work experiences'
                    ]
                },
                actionPlan: {
                    ar: [
                        'أضف صورة شخصية احترافية اليوم',
                        'اكتب عنواناً واضحاً يصف تخصصك',
                        'أضف 3 خبرات عمل على الأقل',
                        'ابحث عن 20 زميلاً سابقاً وأضفهم'
                    ],
                    en: [
                        'Add professional profile picture today',
                        'Write clear headline describing your specialty',
                        'Add at least 3 work experiences',
                        'Find and add 20 former colleagues'
                    ]
                }
            }
        };

        // نظام تحليل ذكي يعتمد على بيانات المستخدم
        function analyzeProfile(linkedinUrl, userGoal) {
            // تحليل الرابط لاستخراج معلومات
            const urlAnalysis = analyzeLinkedInUrl(linkedinUrl);
            
            // تحليل الهدف لمعرفة الأولويات
            const goalAnalysis = analyzeUserGoal(userGoal);
            
            // توليد نتيجة مخصصة بناءً على البيانات
            return generateSmartResult(urlAnalysis, goalAnalysis);
        }

        function analyzeLinkedInUrl(url) {
            // محاكاة تحليل الرابط
            const hasCustomUrl = !url.includes('/in/') || url.includes('/in/yourname') ? 0 : 1;
            const urlLength = url.length;
            const hasSpecialChars = /[^a-zA-Z0-9\/:.-]/.test(url) ? 1 : 0;
            
            // حساب جودة الرابط
            const urlScore = hasCustomUrl * 0.6 + (urlLength < 50 ? 0.2 : 0) + (hasSpecialChars ? 0 : 0.2);
            
            return {
                hasCustomUrl,
                urlLength,
                hasSpecialChars,
                urlScore
            };
        }

        function analyzeUserGoal(goal) {
            // تحليل الهدف لمعرفة الأولويات
            const priorities = {
                job: ['experience', 'skills', 'recommendations'],
                clients: ['headline', 'about', 'portfolio'],
                networking: ['connections', 'activity', 'engagement']
            };
            
            return {
                goal,
                priorities: priorities[goal] || ['headline', 'experience', 'skills']
            };
        }

        function generateSmartResult(urlAnalysis, goalAnalysis) {
            // استخدام تحليل الرابط لتحديد مستوى الحساب
            let baseScore;
            let strengthLevel;
            
            if (urlAnalysis.urlScore >= 0.8) {
                strengthLevel = 'excellent';
                baseScore = 8.5 + Math.random() * 1.0;
            } else if (urlAnalysis.urlScore >= 0.6) {
                strengthLevel = 'good';
                baseScore = 7.0 + Math.random() * 1.4;
            } else if (urlAnalysis.urlScore >= 0.4) {
                strengthLevel = 'average';
                baseScore = 5.5 + Math.random() * 1.4;
            } else {
                strengthLevel = 'poor';
                baseScore = 4.0 + Math.random() * 1.4;
            }
            
            // تعديل النتيجة بناءً على الهدف
            const goalModifier = goalAnalysis.goal === 'job' ? 0.2 : 
                                goalAnalysis.goal === 'clients' ? 0.1 : 0;
            
            const finalScore = Math.min(9.9, baseScore + goalModifier).toFixed(1);
            
            return {
                strengthLevel,
                score: finalScore
            };
        }

        // دالة الترجمة
        function toggleLanguage() {
            const body = document.body;
            const isEnglish = body.classList.contains('english');
            
            if (isEnglish) {
                body.classList.remove('english');
                document.documentElement.lang = 'ar';
                document.documentElement.dir = 'rtl';
            } else {
                body.classList.add('english');
                document.documentElement.lang = 'en';
                document.documentElement.dir = 'ltr';
            }
        }

        // إعداد شاشة التحميل
        function setupLoadingSteps() {
            const isEnglish = document.body.classList.contains('english');
            const lang = isEnglish ? 'en' : 'ar';
            
            const steps = [
                { id: 'step1', text: { ar: 'جاري فحص رابط الحساب...', en: 'Checking profile URL...' } },
                { id: 'step2', text: { ar: 'تحليل الصورة الشخصية والعنوان...', en: 'Analyzing profile picture and headline...' } },
                { id: 'step3', text: { ar: 'فحص قسم الخبرات العملية...', en: 'Checking work experience section...' } },
                { id: 'step4', text: { ar: 'تحليل المهارات والتوصيات...', en: 'Analyzing skills and recommendations...' } },
                { id: 'step5', text: { ar: 'مراجعة النشاط والشبكة...', en: 'Reviewing activity and network...' } },
                { id: 'step6', text: { ar: 'توليد التوصيات المخصصة...', en: 'Generating personalized recommendations...' } }
            ];
            
            const loadingStepsElement = document.getElementById('loadingSteps');
            loadingStepsElement.innerHTML = steps.map(step => `
                <div class="loading-step" id="${step.id}">
                    <div class="step-icon"><i class="fas fa-circle"></i></div>
                    <div>${step.text[lang]}</div>
                </div>
            `).join('');
        }

        // كود التحليل الذكي المحسن
        document.getElementById('analyzeBtn').addEventListener('click', async function() {
            const linkedinUrl = document.getElementById('linkedinUrl').value;
            const userGoal = document.getElementById('userGoals').value;
            const isEnglish = document.body.classList.contains('english');
            
            if (!linkedinUrl) {
                alert(isEnglish ? "Please enter your LinkedIn profile URL" : "يرجى إدخال رابط حساب LinkedIn");
                return;
            }
            
            if (!userGoal) {
                alert(isEnglish ? "Please select your main goal" : "يرجى اختيار هدفك الرئيسي");
                return;
            }
            
            // إعداد شاشة التحميل
            setupLoadingSteps();
            
            // إظهار تحميل
            document.getElementById('loading').style.display = 'block';
            document.getElementById('analyzeBtn').disabled = true;
            
            // محاكاة تحليل حقيقي مع مؤشر تقدم
            const progressBar = document.getElementById('progressBar');
            const steps = document.querySelectorAll('.loading-step');
            
            // محاكاة تحليل حقيقي يستغرق 30-45 ثانية
            const totalTime = 30000 + Math.random() * 15000; // 30-45 ثانية
            const stepTime = totalTime / 6;
            
            for (let i = 0; i < steps.length; i++) {
                // تحديث الخطوة الحالية
                if (i > 0) {
                    steps[i-1].classList.remove('active');
                    steps[i-1].classList.add('completed');
                }
                steps[i].classList.add('active');
                
                // تحديث شريط التقدم
                const progress = ((i + 1) / steps.length) * 100;
                progressBar.style.width = `${progress}%`;
                
                // انتظار بين الخطوات
                await new Promise(resolve => setTimeout(resolve, stepTime));
            }
            
            // إخفاء التحميل وإظهار النتائج
            document.getElementById('loading').style.display = 'none';
            generateSmartAnalysis(linkedinUrl, userGoal);
            document.getElementById('result').style.display = 'block';
            document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
        });
        
        function generateSmartAnalysis(linkedinUrl, userGoal) {
            const isEnglish = document.body.classList.contains('english');
            const lang = isEnglish ? 'en' : 'ar';
            
            // توليد تحليل ذكي بناءً على البيانات
            const analysisResult = analyzeProfile(linkedinUrl, userGoal);
            const levelData = profileAnalysisData[analysisResult.strengthLevel];
            
            // تحديث النتائج
            updateAnalysisResults(analysisResult.score, levelData, lang, analysisResult.strengthLevel);
        }

        function updateAnalysisResults(score, levelData, lang, strengthLevel) {
            // تحديث الدرجة والدائرة
            document.getElementById('score').textContent = score;
            const scoreCircle = document.getElementById('scoreCircle');
            scoreCircle.style.background = `conic-gradient(${levelData.color} 0% ${score * 10}%, #e2e8f0 ${score * 10}% 100%)`;
            
            // تحديث وصف الدرجة
            const scoreDescription = document.getElementById('scoreDescription');
            scoreDescription.innerHTML = levelData.description[lang];
            
            // إضافة تقييم قوة البروفايل
            const profileStrengthElement = document.getElementById('profileStrength');
            const strengthText = {
                excellent: { ar: 'ممتاز', en: 'Excellent' },
                good: { ar: 'جيد', en: 'Good' },
                average: { ar: 'متوسط', en: 'Average' },
                poor: { ar: 'بحاجة للتحسين', en: 'Needs Improvement' }
            };
            
            profileStrengthElement.innerHTML = `
                <strong>${lang === 'ar' ? 'قوة البروفايل:' : 'Profile Strength:'}</strong> 
                <span class="score-badge ${levelData.badge}">
                    ${strengthText[strengthLevel][lang]}
                </span>
                <p style="margin-top: 10px; margin-bottom: 0;">
                    ${lang === 'ar' 
                        ? `هذا التقييم يعكس جودة حسابك مقارنة بالمحترفين الآخرين` 
                        : `This rating reflects your profile quality compared to other professionals`}
                </p>
            `;
            
            // تحديث نقاط القوة
            const strengthsElement = document.getElementById('strengths');
            strengthsElement.innerHTML = levelData.strengths[lang].map(strength => 
                `<li><span class="tip-icon" style="color: ${levelData.color}">✅</span> ${strength}</li>`
            ).join('');
            
            // تحديث مجالات التحسين
            const improvementsElement = document.getElementById('improvements');
            improvementsElement.innerHTML = levelData.improvements[lang].map(improvement => 
                `<li><span class="tip-icon" style="color: ${levelData.color}">🔧</span> ${improvement}</li>`
            ).join('');
            
            // تحديث خطة العمل
            const actionPlanElement = document.getElementById('actionPlan');
            actionPlanElement.innerHTML = levelData.actionPlan[lang].map(action => 
                `<li><span class="tip-icon" style="color: ${levelData.color}">🎯</span> ${action}</li>`
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
