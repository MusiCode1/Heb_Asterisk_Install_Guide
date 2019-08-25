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
```
sudo apt -y install git curl wget libnewt-dev libssl-dev libncurses5-dev subversion  libsqlite3-dev build-essential libjansson-dev libxml2-dev  uuid-dev
```
