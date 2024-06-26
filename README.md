# samparka
* An official Python Package on Pypi.org

Prints the email and the phone number from the website.
Phone number is available for Nepal & USA as of now

Developed by Ujjawal Shah (c) 2024

## Examples of How To Use Package

### Get contact email from the website homepage

```python
import samparka

homepage = samparka.Scrollhomepage('https://howard.edu/')
email_adresses = homepage.emails()
print(f'emails: {email_adresses}')
```
**Output**:

***emails: ['admission@howard.edu', 'hugsadmission@howard.edu']***

### Get phonenumbers from the homepage

```python
import samparka

#to see which countries are available for the phone numbers
print(samparka.__availablecountries__)
```
**Output**:

***['Nepal', 'USA']***


```python
import samparka

homepage = samparka.Scrollhomepage('https://howard.edu/')
phone_numbers = homepage.phonenumbers('USA')
print(f'phone_numbers: {phone_numbers}')
```
**Output**:

***phone_numbers: ['202-806-2763', '202-806-4465', '202-865-6100', '3341862722', '202-806-2755', '202-806-6800', '202-806-6100', '1-800-822-6363']***


```python
import samparka

homepage = samparka.Scrollhomepage('https://www.setopati.com/')
phone_numbers = homepage.phonenumbers('Nepal')
print(f'phone_numbers: {phone_numbers}')
```
**Output**:

***['+977-1-5429319', '9741857838', '9772067662', '9771494820', '9703857991', '9823847051', '9839993648', '9644041575', '9801123339', '9872264189', '9873538472', '9860830966', '9830826490', '+977-1-5428194', '9731283648', '9652935037', '9702006458', '9851123339']***
