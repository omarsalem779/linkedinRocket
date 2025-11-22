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
            --danger: #dc3545;
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

        /* باقي الCSS يبقى كما هو */
        /* ... */

        .score-badge {
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: bold;
            margin-top: 10px;
            display: inline-block;
        }

        .score-excellent { background: var(--success); color: white; }
        .score-good { background: var(--warning); color: black; }
        .score-average { background: #ff9800; color: white; }
        .score-poor { background: var(--danger); color: white; }

        .profile-strength {
            margin: 15px 0;
            padding: 15px;
            border-radius: 10px;
            background: #f8f9fa;
            border-right: 4px solid var(--primary);
        }

    </style>
</head>
<body>
    <!-- باقي الهيكل يبقى كما هو -->
    <!-- ... -->

    <script>
        // قاعدة بيانات النصائح حسب مستوى القوة
        const analysisData = {
            excellent: {
                score: { min: 8.5, max: 10 },
                strengths: {
                    ar: [
                        'صورة شخصية احترافية ومميزة جداً',
                        'العنوان يوضح تخصصك وقيمتك بشكل ممتاز',
                        'شبكة تواصل قوية ومتنوعة مع محترفين',
                        'الخبرات موثقة بإنجازات رقمية ملموسة',
                        'قسم المهارات شامل ويحتوي على توصيات',
                        'التفاعل المستمر مع المحتوى في مجالك'
                    ],
                    en: [
                        'Exceptional professional profile picture',
                        'Headline perfectly showcases your expertise and value',
                        'Strong and diverse network of professionals',
                        'Experiences documented with tangible digital achievements',
                        'Comprehensive skills section with endorsements',
                        'Consistent engagement with industry content'
                    ]
                },
                improvements: {
                    ar: [
                        'فكر في إنشاء محتوى فيديو لتوسيع تأثيرك',
                        'انضم إلى مجموعات متخصصة وكن نشطاً فيها',
                        'اطلب توصيات من قادة في مجالك',
                        'أنشئ مدونة على LinkedIn لمشاركة خبراتك',
                        'استخدم hashtags استراتيجية في منشوراتك'
                    ],
                    en: [
                        'Consider creating video content to expand your reach',
                        'Join specialized groups and be active in them',
                        'Request recommendations from industry leaders',
                        'Start a LinkedIn blog to share your expertise',
                        'Use strategic hashtags in your posts'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى قيماً 3 مرات أسبوعياً',
                        'تفاعل مع 10 منشورات يومياً في مجالك',
                        'ارسل 5 طلبات اتصال أسبوعياً لمحترفين جدد',
                        'اكتب مقالة واحدة شهرياً على LinkedIn',
                        'حضر فعاليتين افتراضيتين شهرياً'
                    ],
                    en: [
                        'Post valuable content 3 times per week',
                        'Engage with 10 posts daily in your industry',
                        'Send 5 connection requests weekly to new professionals',
                        'Write one monthly article on LinkedIn',
                        'Attend two virtual events monthly'
                    ]
                }
            },
            good: {
                score: { min: 7.0, max: 8.4 },
                strengths: {
                    ar: [
                        'صورة شخصية احترافية ومناسبة',
                        'العنوان يوضح تخصصك بشكل جيد',
                        'شبكة تواصل جيدة ولكن يمكن توسعتها',
                        'الخبرات موثقة بشكل واضح',
                        'قسم المهارات يحتوي على مهارات رئيسية'
                    ],
                    en: [
                        'Professional and appropriate profile picture',
                        'Headline clearly shows your specialization',
                        'Good network but could be expanded',
                        'Experiences are clearly documented',
                        'Skills section contains key competencies'
                    ]
                },
                improvements: {
                    ar: [
                        'أضف صورة غلاف تعبر عن هويتك المهنية',
                        'طور قسم About ليكون أكثر إقناعاً',
                        'اطلب المزيد من التوصيات للخبرات',
                        'أضف مشاريع شخصية إلى حسابك',
                        'زد تفاعلك مع محتوى الآخرين'
                    ],
                    en: [
                        'Add a cover photo reflecting your professional identity',
                        'Enhance About section to be more compelling',
                        'Request more recommendations for experiences',
                        'Add personal projects to your profile',
                        'Increase engagement with others content'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى قيماً مرتين أسبوعياً',
                        'تفاعل مع 7 منشورات يومياً',
                        'اطلب توصيتين هذا الأسبوع',
                        'حدث قسم المشاريع الشخصية',
                        'انضم إلى 3 مجموعات متخصصة'
                    ],
                    en: [
                        'Post valuable content twice weekly',
                        'Engage with 7 posts daily',
                        'Request 2 recommendations this week',
                        'Update personal projects section',
                        'Join 3 specialized groups'
                    ]
                }
            },
            average: {
                score: { min: 5.0, max: 6.9 },
                strengths: {
                    ar: [
                        'صورة شخصية واضحة ولكن تحتاج تحسين',
                        'العنوان أساسي ولكن يمكن تطويره',
                        'شبكة تواصل أساسية',
                        'الخبرات مسجلة ولكن تحتاج تفصيل'
                    ],
                    en: [
                        'Clear profile picture but needs improvement',
                        'Basic headline that can be enhanced',
                        'Basic network of connections',
                        'Experiences recorded but need detailing'
                    ]
                },
                improvements: {
                    ar: [
                        'غير صورتك الشخصية لصورة أكثر احترافية',
                        'أعد كتابة العنوان ليكون أكثر جاذبية',
                        'أضف وصفاً مفصلاً لكل خبرة عمل',
                        'طور قسم المهارات بإضافة 10 مهارات على الأقل',
                        'ابدأ في التفاعل مع المحتوى بانتظام'
                    ],
                    en: [
                        'Change profile picture to more professional one',
                        'Rewrite headline to be more attractive',
                        'Add detailed description for each work experience',
                        'Enhance skills section with at least 10 skills',
                        'Start engaging with content regularly'
                    ]
                },
                actionPlan: {
                    ar: [
                        'انشر محتوى مرة أسبوعياً على الأقل',
                        'تفاعل مع 5 منشورات يومياً',
                        'أكمل قسم About بشكل مفصل',
                        'أضف 3 مهارات جديدة هذا الأسبوع',
                        'اطلب توصية واحدة على الأقل'
                    ],
                    en: [
                        'Post content at least once weekly',
                        'Engage with 5 posts daily',
                        'Complete About section in detail',
                        'Add 3 new skills this week',
                        'Request at least one recommendation'
                    ]
                }
            },
            poor: {
                score: { min: 0, max: 4.9 },
                strengths: {
                    ar: [
                        'لديك حساب LinkedIn - هذه بداية جيدة',
                        'يمكنك البدء في بناء وجودك المهني'
                    ],
                    en: [
                        'You have a LinkedIn account - good start',
                        'You can start building your professional presence'
                    ]
                },
                improvements: {
                    ar: [
                        'أضف صورة شخصية احترافية فوراً',
                        'اكتب عنواناً يوضح تخصصك وهدفك',
                        'املأ قسم About بشكل كامل',
                        'أضف خبراتك العملية السابقة',
                        'ابدأ في بناء شبكة تواصل أساسية'
                    ],
                    en: [
                        'Add professional profile picture immediately',
                        'Write headline showing your specialty and goal',
                        'Fill About section completely',
                        'Add your previous work experiences',
                        'Start building basic network'
                    ]
                },
                actionPlan: {
                    ar: [
                        'أضف صورة شخصية احترافية اليوم',
                        'اكتب عنواناً جذاباً يصفك',
                        'أضف 3 خبرات عمل على الأقل',
                        'ابحث عن 10 زملاء سابقين وأضفهم',
                        'ابدأ بمشاهدة المحتوى في مجالك'
                    ],
                    en: [
                        'Add professional profile picture today',
                        'Write attractive headline describing you',
                        'Add at least 3 work experiences',
                        'Find and add 10 former colleagues',
                        'Start viewing content in your industry'
                    ]
                }
            }
        };

        // دالة لتقييم قوة البروفايل بشكل عشوائي ولكن واقعي
        function assessProfileStrength(linkedinUrl) {
            // محاكاة تحليل حقيقي للبروفايل
            const randomFactor = Math.random();
            let strengthLevel;
            
            if (randomFactor < 0.15) {
                strengthLevel = 'excellent'; // 15% من الحسابات ممتازة
            } else if (randomFactor < 0.45) {
                strengthLevel = 'good'; // 30% من الحسابات جيدة
            } else if (randomFactor < 0.80) {
                strengthLevel = 'average'; // 35% من الحسابات متوسطة
            } else {
                strengthLevel = 'poor'; // 20% من الحسابات ضعيفة
            }
            
            return strengthLevel;
        }

        // دالة لتوليد درجة عشوائية ضمن النطاق
        function generateRandomScore(min, max) {
            return (Math.random() * (max - min) + min).toFixed(1);
        }

        // دالة الترجمة المحسنة
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

        // كود التحليل الذكي
        document.getElementById('analyzeBtn').addEventListener('click', function() {
            const linkedinUrl = document.getElementById('linkedinUrl').value;
            const userGoals = document.getElementById('userGoals').value;
            const isEnglish = document.body.classList.contains('english');
            
            if (!linkedinUrl) {
                alert(isEnglish ? "Please enter your LinkedIn profile URL" : "يرجى إدخال رابط حساب LinkedIn");
                return;
            }
            
            // إظهار تحميل
            document.getElementById('loading').style.display = 'block';
            document.getElementById('analyzeBtn').disabled = true;
            
            // محاكاة اتصال بالذكاء الاصطناعي
            setTimeout(() => {
                document.getElementById('loading').style.display = 'none';
                generateSmartAnalysis(linkedinUrl, userGoals);
                document.getElementById('result').style.display = 'block';
                document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
            }, 2000);
        });
        
        function generateSmartAnalysis(url, goals) {
            const isEnglish = document.body.classList.contains('english');
            const lang = isEnglish ? 'en' : 'ar';
            
            // تقييم قوة البروفايل
            const strengthLevel = assessProfileStrength(url);
            const levelData = analysisData[strengthLevel];
            
            // توليد درجة عشوائية ضمن النطاق
            const score = generateRandomScore(levelData.score.min, levelData.score.max);
            
            // عرض النتائج
            document.getElementById('score').textContent = score;
            
            // تحديث لون الدائرة حسب الدرجة
            const scoreCircle = document.querySelector('.score-circle');
            scoreCircle.style.background = `conic-gradient(${getScoreColor(score)} 0% ${score * 10}%, #e2e8f0 ${score * 10}% 100%)`;
            
            // إضافة تقييم نصي
            const scoreText = document.querySelector('.score-container > div > p');
            scoreText.innerHTML = getScoreDescription(score, lang);
            
            // عرض نقاط القوة
            const strengthsElement = document.getElementById('strengths');
            strengthsElement.innerHTML = levelData.strengths[lang].map(strength => 
                `<li><span class="tip-icon">✅</span> ${strength}</li>`
            ).join('');
            
            // عرض مجالات التحسين
            const improvementsElement = document.getElementById('improvements');
            improvementsElement.innerHTML = levelData.improvements[lang].map(improvement => 
                `<li><span class="tip-icon">🔧</span> ${improvement}</li>`
            ).join('');
            
            // عرض خطة العمل
            const actionPlanElement = document.getElementById('actionPlan');
            actionPlanElement.innerHTML = levelData.actionPlan[lang].map(action => 
                `<li><span class="tip-icon">🎯</span> ${action}</li>`
            ).join('');

            // إضافة نص قوة البروفايل
            const profileStrengthElement = document.createElement('div');
            profileStrengthElement.className = 'profile-strength';
            profileStrengthElement.innerHTML = `
                <strong>${isEnglish ? 'Profile Strength:' : 'قوة البروفايل:'}</strong> 
                <span class="score-badge ${getScoreBadgeClass(score)}">
                    ${getStrengthLevelText(strengthLevel, lang)}
                </span>
            `;
            document.querySelector('.score-container').appendChild(profileStrengthElement);
        }

        // دوال مساعدة
        function getScoreColor(score) {
            if (score >= 8.5) return 'var(--success)';
            if (score >= 7.0) return 'var(--warning)';
            if (score >= 5.0) return '#ff9800';
            return 'var(--danger)';
        }

        function getScoreBadgeClass(score) {
            if (score >= 8.5) return 'score-excellent';
            if (score >= 7.0) return 'score-good';
            if (score >= 5.0) return 'score-average';
            return 'score-poor';
        }

        function getScoreDescription(score, lang) {
            if (score >= 8.5) {
                return lang === 'ar' 
                    ? 'ممتاز - حسابك من أفضل الحسابات المهنية'
                    : 'Excellent - Your profile is among the top professional accounts';
            } else if (score >= 7.0) {
                return lang === 'ar'
                    ? 'جيد جداً - يمكنك التحسين إلى مستوى ممتاز'
                    : 'Very Good - You can improve to excellent level';
            } else if (score >= 5.0) {
                return lang === 'ar'
                    ? 'متوسط - لديك أساس جيد يحتاج تطوير'
                    : 'Average - You have a good foundation that needs development';
            } else {
                return lang === 'ar'
                    ? 'يحتاج تحسين - ابدأ في بناء حسابك المهني'
                    : 'Needs Improvement - Start building your professional profile';
            }
        }

        function getStrengthLevelText(level, lang) {
            const levels = {
                excellent: { ar: 'ممتاز', en: 'Excellent' },
                good: { ar: 'جيد', en: 'Good' },
                average: { ar: 'متوسط', en: 'Average' },
                poor: { ar: 'ضعيف', en: 'Poor' }
            };
            return levels[level][lang];
        }

        // زر تحليل جديد
        document.getElementById('newAnalysis').addEventListener('click', function() {
            document.getElementById('linkedinUrl').value = '';
            document.getElementById('userGoals').value = '';
            document.getElementById('result').style.display = 'none';
            document.getElementById('analyzeBtn').disabled = false;
            
            // إزالة نص قوة البروفايل المضاف
            const existingStrengthElement = document.querySelector('.profile-strength');
            if (existingStrengthElement) {
                existingStrengthElement.remove();
            }
            
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });

        // زر LinkedIn
        document.querySelector('.btn-expert').addEventListener('click', function(e) {
            e.preventDefault();
            window.open('https://www.linkedin.com/in/omarsalem779', '_blank');
        });
    </script>
</body>
</html>
