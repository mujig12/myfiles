$EmailFrom = “bnmauddda@gmail.com”

$EmailTo = “bnmauddda@gmail.com”

$Subject = “Test”

$Body = “Tricknology Test”

$SMTPServer = “smtp.gmail.com”

$SMTPClient = New-Object Net.Mail.SmtpClient($SmtpServer, 587)

$SMTPClient.EnableSsl = $true

$SMTPClient.Credentials = New-Object System.Net.NetworkCredential(“bnmauddda@gmail.com”, “Mjl45134”);
$SMTPClient.Send($EmailFrom, $EmailTo, $Subject, $Body)