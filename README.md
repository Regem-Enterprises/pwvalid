
# PWValid Email Validation 

PWValid is a powerful and very simple Python package to validate and check emails. It helps developers tackle spam and disposable emails.



### Features:
+ Fast Response
+ Very Accurate
+ Easy to Implement
+ No Need to use External APIs
+ No Need for Any API Key

### Installation
**Pip Command**

```
pip install pwvalid
```

### How to use?

**Import pwvalid Package**

```
import pwvalid
```

### InBuilt Functions:
#### EmailValidate Fuction:
It checks and validates the emails and returns a complete response with all available metrics.

```
pwvalid.EmailValidate('youremail@gmail.com')
```


#### Avaliable Metrics
```
result = pwvalid.EmailValidate('youremail@gmail.com')
```
+ _email_address_ : `result['email_address']` | Response Type: String
+ _domain_ : `result['domain']` | Response Type: String
+ _disposables_ : `result['disposable']` | Response Type: Bool
+ _webmails_ : `result['webmail']` | Response Type: Bool
+ _deliverable_ : `result['deliverable']` | Response Type: Bool
+ _valid_syntax_ : `result['valid_syntax']` | Response Type: Bool
+ _catch_all_ : `result['catch_all']` | Response Type: Bool
+ _gibberish_ : `result['gibberish']` | Response Type: Bool
+ _spam_ : `result['spam']` | Response Type: Bool

Example Response:

```
{
  'email_address': 'kush@gmail.com',
  'domain': 'gmail.com',
  'valid_syntax': True,
  'disposable': False,
  'webmail': True,
  'deliverable': False,
  'catch_all': False,
  'gibberish': False,
  'spam': False
}
```


---
#### isDisposable Fuction:
It checks if an email is disposable or not. It returns a boolean response (True/False).

```
pwvalid.isDisposable('youremail@gmail.com')
```

---
#### isDeliverable Fuction:
It Checks if an email is Deliverable or not. it returns a Bool response. (True/False)

```
pwvalid.isDeliverable('youremail@gmail.com')
```

---
#### isSpam Fuction:
It Checks if an email is Spam or not. it returns a Bool response. (True/False)

```
pwvalid.isSpam('youremail@gmail.com')
```

---

### Code Examples
```
import pwvalid 
email = input('Enter Email:')
result = pwvalid.isSpam(email)
print(result)
```

### Support This Project
[![paypal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/itsvinaychaudhary) 

[![coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/vinay_dev)

### Author
The PWValid Package is created by [Vinay Chaudhary](https://buymeacoffee.com/vinay_dev). This Project is Powered by [Regem Enterprises](https://regem.in)
