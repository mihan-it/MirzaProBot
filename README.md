## ⭐ لطفاً پروژه را **Star** کنید تا دیگران هم آن را پیدا کنند!


---

 #### **💸  حمایت مالی**


<details>
  <summary> دونیت </summary>

👉 [حمایت از دولوپر میرزا NowPayments](https://nowpayments.io/donation/permiumbotmirza)



  

</details>




#### **↩️  آموزش نصب اسکریپت در سرور ( Ubuntu 24 )**


<details>
  <summary> نصب سرور خام  </summary>

  #### 1️⃣ ابتدا دستور آپدیت و آپگرید را اجرا کرده و سپس اسکریپت زیر را بر روی سرور اجرا کنید.
 ```
  bash -c "$(curl -L https://raw.githubusercontent.com/mihan-it/MirzaProBot/main/install.sh)"
```

#### 2️⃣ سپس گزینهٔ «1» را انتخاب کرده و اطلاعات مورد نیاز را مطابق درخواست وارد نمایید.
#### 3️⃣ مجددا اسکریپت را اجرا کرده و گزینهٔ 10 را انتخاب کنید تا مجوزهای مربوط به فایل‌ها به‌صورت خودکار تنظیم شود.
#### 4️⃣ پس از اتمام کار، با زدن گزینه 11 از اسکریپت خارج شوید و برای حذف فایل (Installer) دستور زیر را اجرا کنید:

```
rm -r /var/www/html/mirzabotconfig/installer
```

### ⛔️حذف فایل Installer الزامی است.
</details>

---





#### **📊  اطلاعات کلی**


<details>
  <summary> توضیحات </summary>


---

| php | کرون جاب | 
|--------|------|
| 8.3 / 8.4  | اجباری |

پس از نصب با زدن دستور crontab -e کرون جاب های زیر را قرار داده و ذخیره نمائید :

* * * * * php /var/www/html/mirzaprobotconfig/cronbot/NoticationsService.php >/dev/null 2>&1
*/5 * * * * php /var/www/html/mirzaprobotconfig/cronbot/uptime_panel.php >/dev/null 2>&1
*/5 * * * * php /var/www/html/mirzaprobotconfig/cronbot/uptime_node.php >/dev/null 2>&1
*/10 * * * * php /var/www/html/mirzaprobotconfig/cronbot/expireagent.php >/dev/null 2>&1
*/10 * * * * php /var/www/html/mirzaprobotconfig/cronbot/payment_expire.php >/dev/null 2>&1
0 * * * * php /var/www/html/mirzaprobotconfig/cronbot/statusday.php >/dev/null 2>&1
0 3 * * * php /var/www/html/mirzaprobotconfig/cronbot/backupbot.php >/dev/null 2>&1
*/15 * * * * php /var/www/html/mirzaprobotconfig/cronbot/iranpay1.php >/dev/null 2>&1
*/15 * * * * php /var/www/html/mirzaprobotconfig/cronbot/plisio.php >/dev/null 2>&1

  
</details>


