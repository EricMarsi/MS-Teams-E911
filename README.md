# MS-Teams-E911
MS Teams E911 Repo

Just a bunch of files that helps with deploying 911 in Microsoft Teams

Here's some commands as well that will help with filling GUIDs in the Excel import file

#Civic Address
Get-CsOnlineLisCivicAddress | Select Description,CivicAddressID,DefaultLocationID | Export-Csv -NoTypeInformation -Path .\desktop\Civic.csv

#LocationIDs
Get-CsOnlineLisLocation | Select Description,CivicAddressID,Location,LocationID | Export-Csv -NoTypeInformation -Path .\desktop\Loc.csv

