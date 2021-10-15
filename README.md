DataSet
https://www.kaggle.com/muhammadshahzadkhan/dogvscat

OPEN PowerShell and Test your WebAPI
$body = @{ImageSource = <Image location on your local machine>

Invoke-RestMethod "https://localhost:<PORT>/predict" -Method Post -Body ($body | ConvertTo-Json) -ContentType "application/json"
