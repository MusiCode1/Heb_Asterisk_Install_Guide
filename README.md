# Heb_Asterisk_Install_Guide
The first online guide to installing Asterisk and FreePBX in Hebrew!
<div dir="rtl">
שימו לב:
בקובץ זה, לא נתתי דגש על לעשות את הדברים מהר, אלא להבין כל פקודה, כמה שאפשר, מה היא מבצעת.
בהרבה מקרים ניתן לבצע את הפעולות מהר יותר.

# מדריך התקנת מרכזיית אסטריסק מקבצי המקור

## התקנת אסטריסק

### התקנת תלויות

נתקין את כל החבילות שאסטריסק צריכה לפעולה תקינה:
<div dir="ltr">

```
sudo apt -y install git curl wget libnewt-dev libssl-dev libncurses5-dev subversion  libsqlite3-dev build-essential libjansson-dev libxml2-dev  uuid-dev
```
<div dir="rtl">
אם מתקבלת הודעת שגיאה על חבילת subversion, כזאת:
```
E: Package 'subversion' has no installation candidate
```

צריך להוסיף את המקור שלה למאגר. כך:
```
sudo add-apt-repository universe
sudo apt update && sudo apt -y install subversion
```
(מקור: https://computingforgeeks.com/how-to-install-asterisk-16-lts-on-ubuntu-18-04-16-04-debian-9/)
