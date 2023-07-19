
# PWValid Email Validation 

PWValid is a Powerful and Verysimple python package to Validate and Check Emails. it helps developer to tackle spam and disposible emails.

### Features:
+ Fast Response
+ Very Accurate
+ Easy to Implement
+ No Need to use External APIs
+ No Need of Any API Key

### Installation
**Pip Command**

`
pip install pwvalid
`

### How to use?

**Import pwvalid Package**

`
import pwvalid
`

### InBuilt Functions:
#### EmailValidate Fuction:
It Checks and Validates the Emails and returns a complete response with all avaliable metrics.

`pwvalid.EmailValidate('youremail@gmail.com')`


#### Avaliable Metrics
`result = pwvalid.EmailValidate('youremail@gmail.com')`
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

`
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
`


---
#### isDisposable Fuction:
It Checks that email is disposible or not. it returns a Bool response. (True/False)

`pwvalid.isDisposable('youremail@gmail.com')`

---
#### isDeliverable Fuction:
It Checks that email is Deliverable or not. it returns a Bool response. (True/False)

`pwvalid.isDeliverable('youremail@gmail.com')`

---
#### isSpam Fuction:
It Checks that email is Spam or not. it returns a Bool response. (True/False)

`pwvalid.isSpam('youremail@gmail.com')`

---

### Code Examples
<code>
import pwvalid 
email = input('Enter Email:')
result = pwvalid.isSpam(email)
print(result)
</code>



