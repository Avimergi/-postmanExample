# -postmansample
this is a postman code sample of isr taxes open api 

דוגמאות Postman
1.	Get token using postman…
   
 זוהי דוגמא לשימוש במנגנון מובנה של פוסטמן לקבלת jwt בפרוטוקול oauth נכנסים לחלונית authorization 
 ![image](https://github.com/ISRTaxesOpenAPI/-postmanExample/assets/121564724/4918e261-5dfd-4e90-89f4-cc9f4f009112)

ממלאים את הפרטים ולוחצים על כפתור ליצירת טוקן

![image](https://github.com/ISRTaxesOpenAPI/-postmanExample/assets/121564724/5bcc56ac-9a15-4ac0-bc3e-b8b5a11127a5)

 מזדהים ומקבלים את ה access token + refresh token

![image](https://github.com/ISRTaxesOpenAPI/-postmanExample/assets/121564724/ef979506-5484-4a50-aca5-779d6421f6e6)

 2.	Refresh token
 מבצעים קריאת post  לכתובת ה token עם הפרמטרים הרלוונטים ב body  אחד מהם הוא ה refresh  שקיבלת בסעיף 1 לדוגמא

 3.	Get authorization code
    
   
פניית get  לקבלת authorization code המשמש להנפקת טוקן (סעיף 4) מזינים ב params  את הערכים הרלוונטים מעתיקים את הכתובת לדפדפן מזדהים ומקבלים את ה code  ב url
   
4. Get token

    קריאת post לכתובת ה token עם הפרמטים הרלוונטים ב body  שאחד מהם הוא  code  (מסעיף 3) חוזר מקריאה זו access token + refresh token זהה לתשובה של 1 . כמובן שפעולות 3-4 זהות ל1 אך כאן ראינו את הפניות עצמם ללא המנגנון האוטומטי של postman
