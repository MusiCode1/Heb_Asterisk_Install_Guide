# Heb_Asterisk_Install_Guide
The first online guide to installing Asterisk and FreePBX in Hebrew!
<div dir="rtl" style="
pre {
  dir: ltr;
}
" >
שימו לב:
בקובץ זה, לא נתתי דגש על לעשות את הדברים מהר, אלא להבין כל פקודה, כמה שאפשר, מה היא מבצעת.
בהרבה מקרים ניתן לבצע את הפעולות מהר יותר.

# מדריך התקנת מרכזיית אסטריסק מקבצי המקור

## התקנת אסטריסק

### התקנת תלויות

נתקין את כל החבילות שאסטריסק צריכה לפעולה תקינה:

```bash
sudo apt -y install git curl wget libnewt-dev libssl-dev libncurses5-dev subversion  libsqlite3-dev build-essential libjansson-dev libxml2-dev  uuid-dev
```

אם מתקבלת הודעת שגיאה על חבילת subversion, כזאת:
```bash {:custom-id}
E: Package 'subversion' has no installation candidate
```

צריך להוסיף את המקור שלה למאגר. כך:
```bash
sudo add-apt-repository universe
sudo apt update && sudo apt -y install subversion
```
(מקור: https://computingforgeeks.com/how-to-install-asterisk-16-lts-on-ubuntu-18-04-16-04-debian-9/)

### הורדת הגרסה האחרונה
קודם נוריד את הגרסה האחרונה (עם תמיכה לטווח ארוך - TLS) של אסטריסק:
> הגרסה האחרונה נכון לעכשיו היא 16.

נדפדף לתיקיית scr:
```bash 
cd /usr/src/
```
