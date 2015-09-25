# Print Recruitment Letters and Labels

## Log onto PSYCMORMC014

### Letter Mail Merge
- Open Recruitment Letter in Word  
  - Recruitment letter is located:  
  - Select: Tools > Mail Merge Manager
    1. Create New > Form Letters 
    2. Get List > Open Data Source  
       - Select Excel List  
         - This file may not already be open  
    3. Insert Place Holders  
       - Drag Excel header column title into word document  
         - PFirstName, CFirstName, CLastName
    4. Filter Recipients
       - Options
       - Field: Contact_with_FF
       - Comparison: Equal to
       - Compare to: YES or NO
    5. Complete Merge
       - Merge to a new document
       - Print document
    
### Label Mail Merge
- Open blank Word document   
  - Select: Tools > Mail Merge Manager
    1. Create New > Labels
       - Laser and INk Jet  
       - Avery Standard  
       - 5160-address  
       - OK  
    2. Get List > Open Data Source   
       - Select Excel List  
         - This file may not already be open  
       - Edit Labels Box Opens
    3. Insert Merge Field  
       - Drag each field below into the proper location  
    [PFirstName][PLastName]  
    [Address]  
    [City],[State][Zip]  
    