# 說明使用C#寄送mail之方式
<h2>1.先載入必要package</h2>
<code>using System.Net.Mail;</code><br/>
<code>using System.Net;</code>

<h2>2.產生兩個必要的類別物件</h2>
<code>MailMessage mail = new MailMessage();</code><br/>
<code>SmtpClient smtp = new SmtpClient("SMTP IP-ADDRESS",SMTP PORT);</code>

<h2>3.物件屬性說明</h2>
<code>mail.From = new MailAddress(emailFrom);</code>//寄信郵件帳號<br/>  
<code>mail.To.Add(mailTo);</code>//收信郵件帳號<br/>
<code>mail.Subject = subject;</code>//主旨<br/>
<code>mail.Body = body;</code>//郵件內容<br/>
<code>mail.IsBodyHtml = false;</code>//是否使用HTML格式<br/>
<code>smtp.Credentials = new NetworkCredential(emailFrom, password);</code>//寄信端郵件驗證，有些伺服器需要驗證以防信件仿冒<br/>
<code>smtp.EnableSsl = enableSSL;</code>//是否使用SSL<br/>
<code>smtp.Send(mail);</code>//送出信件<br/>
            


