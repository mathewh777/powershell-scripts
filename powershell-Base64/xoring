$Sa = "Get-PSHost"
$SC = "ProcessInfo"

#$Sa
#$Sb=[Convert]::ToBase64String([Text.encoding]::UTF8.GetBytes($Sa))
#$Sb
#$Sc=[Convert]::FromBase64String("$Sb")
#$Sc
#$Sd=[Text.Encoding]::UTF8.GetString([Convert]::FromBase64String($Sb))
#$Sd
#Test

#Arrays 
$encrypted=@()
$decrypted=@()
#Gets Number for each char
"encrypting "
#BXOR is key 
foreach($byte in [Text.Encoding]::UTF8.GetBytes($SA+$SC)){ "BytesN"; $encrypted; $encrypted += $byte -bxor 116}
#Shrugs
"decrypting" 
foreach($byte in $encrypted){ "BytesN"; $decrypted; $decrypted += $byte -bxor 116}
"Decode"; $decrypted;
"Decoding"; [Text.Encoding]::UTF8.GetString($decrypted)
