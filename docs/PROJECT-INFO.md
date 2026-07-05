<div dir="rtl">

# פרטי הפרויקט — בלשי הצלילים 🔍

**עודכן:** 2026-07-05

## 🌐 האתר החי
- **קישור ישיר:** https://cx-elchanan-arbiv.github.io/balashei-tzlilim/
- **אירוח:** GitHub Pages (חינם, https). המיקרופון עובד שם (עתידי — לסטודיו הקלטות).
- **פועל על:** כל מכשיר/דפדפן. אפשר "הוסף למסך הבית" באייפד/טלפון → נפתח כמו אפליקציה.

## 📦 קוד ומקורות
| מה | היכן | תפקיד |
|---|---|---|
| **מקור-האמת** | `~/Projects/balashei-tzlilim/` | כאן עורכים ומתחזקים |
| **GitHub (repo ציבורי)** | https://github.com/cx-elchanan-arbiv/balashei-tzlilim | חשבון `cx-elchanan-arbiv`; push → האתר מתעדכן |
| עותק מקומי + מפעיל | `~/Documents/בלשי-הצלילים-אפליקציה/` (`הפעלה.command`) | להרצה מקומית עם מיקרופון |
| Artifact | https://claude.ai/code/artifact/b3108a6d-3eaa-4146-9df5-ee2fa5126bcb | ניסיון מהיר (בלי מיקרופון) |

## 🔑 מפתחות שנוצרו
| מפתח | סטטוס | פעולה נדרשת |
|---|---|---|
| **ElevenLabs API — "Stormy Giant Otter"** | נוצר, נוסה, **נמחק מקומית** מ-`~/.elevenlabs_key`. לא בשימוש (ElevenLabs חינם לא מתאים לעברית). | **לבטל אותו ב-ElevenLabs:** Settings → API Keys → מחיקה. |

> אין כרגע אף מפתח פעיל בפרויקט. אם בעתיד נשתמש ב-TTS ענני — המפתח יישמר ב-`~/.<שם>_key` (מוחרג ב-`.gitignore`), **לעולם לא ב-repo**.

## 🚀 תחזוקה
**עריכה → פרסום:**
```
cd ~/Projects/balashei-tzlilim
# עורכים את index.html
git add -A && git commit -m "..." && git push
```
GitHub Pages בונה מחדש (~30ש') → האתר מתעדכן.

**הרצה מקומית (עם מיקרופון):**
```
cd ~/Projects/balashei-tzlilim && python3 -m http.server 8756
# פותחים http://localhost:8756
```

## 🎙️ קול — סטטוס נוכחי
- **כרגע:** בלי קול נוירוני. הקראת-מילים = Carmit (מערכת) **מנוקד**; משוב = **צלילים** (Web Audio).
- **סטודיו הקלטות** קיים בקוד אך **מוסתר** (להחזרה: להוסיף כפתור `#studioBtn` ב-`renderHome`).
- מסלולים פתוחים לקול-עברי טוב: הקלטה-עצמית · Google he-IL Wavenet (ה-GCP שלך) · Azure הילה/אברי.

</div>
