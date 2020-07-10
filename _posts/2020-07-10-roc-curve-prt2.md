---
title: رسم و تفسیر منحنی ROC
data: 2020-07-10
---

<div dir="rtl" lang="fa">
<h1>رسم و تفسیر منحنی ROC</h1>
<p>این بخش ادامه می یابد با مثال کم کاری غده ی تیروئید که در
<a href="https://sohrabkhanbadr.github.io/music-auto-tagging/roc-curve-prt1.html">بخش قبل</a>
شروع شده است. در بخش قبل ما نشان دادیم که جدول زیر یعنی :</p>
<table>
<thead>
<tr>
<th>ستون 1</th>
<th>ستون 2</th>
<th>ستون 3</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>T4 value</strong></td>
<td><strong>Hypothyroid</strong></td>
<td><strong>Euthyroid</strong></td>
</tr>
<tr>
<td>5 or less</td>
<td>18</td>
<td>1</td>
</tr>
<tr>
<td>5.1 - 7</td>
<td>7</td>
<td>17</td>
</tr>
<tr>
<td>7.1 - 9</td>
<td>4</td>
<td>36</td>
</tr>
<tr>
<td>9 or more</td>
<td>3</td>
<td>39</td>
</tr>
<tr>
<td><strong>Totals:</strong></td>
<td>32</td>
<td>93</td>
</tr>
</tbody>
</table>
<p>میتواند خلاصه شود به کمک مشخصه های عملیاتی زیر:</p>
<table>
<thead>
<tr>
<th>ستون 1</th>
<th>ستون 2</th>
<th>ستون 3</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Cutpoint</strong></td>
<td><strong>Sensitivity</strong></td>
<td><strong>Specificity</strong></td>
</tr>
<tr>
<td>5</td>
<td>0.56</td>
<td>0.99</td>
</tr>
<tr>
<td>7</td>
<td>0.78</td>
<td>0.81</td>
</tr>
<tr>
<td>9</td>
<td>0.91</td>
<td>0.42</td>
</tr>
</tbody>
</table>
<p>مشخصه های عملیاتی ذکر شده در بالا میتواند کمی اصلاح شود و سپس به صورت گرافیکی همانطور که در زیر می بینید نشان داده شود.</p>
<p><img src="./assets/uploads/t4roc.jpg" alt="توضیح تصویر"></p>
<p>به این نوع گراف ها <strong>Receiver Operating Characteristic curve</strong> یا منحنی ROC گفته می شود. به فارسی «منحنی مشخصه عملکرد سیستم» نام دارد.این نمودار نرخ مثبت صحیح را در مقابل نرخ مثبت غلط برای برش-cutpoint های ممکن متفاوت از یک آزمایش تشخیصی را نشان می دهد.</p>
<p>منحنی ROC چندین چیز را به تصویر می کشد:</p>
<ol>
<li>این منحنی رابطه ی بین حساسیت و ویژگی-specificity را نشان میدهد(هر افزایشی با حساسیت همراه است با کاهش مشخصات-specificity).</li>
<li>اگر با محور های x و y این نمودار یک مستطیل بسازید ، به فضای ایجاد شده فضای  ROC می گویند. هرچه منحنی از مرز سمت چپ و سپس مرز بالای فضای ROC پیروی کند ، آزمایش دقیق تر است.</li>
<li>هرچه منحنی به مورب 45 درجه ای(قطرای که از مبدا مختصات می گذرد) از فضای ROC نزدیک شود ، آزمایش از دقت پایین تری برخوردار است.</li>
<li>شیب خط مماس بر نقاط برش - cutpoint نرخ درست نمایی-likelihood را نشان میدهد. برای نمونه در گراف بالا نرخ درستنمایی برای  T4&lt;5 برابر با 52 است. نرخ درستنمایی  برای T4&gt;9 برابر با 0.2 است.</li>
<li>ناحیه ی زیر منحنی یک معیار دقت است که در بخش بعد به آن خواهیم پرداخت.</li>
</ol>
</div>
