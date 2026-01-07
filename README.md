# My First Python Project: Caesar Cipher 🔐

**October 2025** - Started learning Python from zero  
**This project** - My first complete program ever  
**Now** - Building cloud security skills

## 🎯 What This Is
This Caesar Cipher encryption program is the **first real code I ever wrote** in Python.

I built this while taking my first Python course in October 2025, with no prior programming experience.

## 💻 The Actual Code I Wrote
```python
def getDoubleAlphabet(alphabet):
    doubleAlphabet = alphabet + alphabet
    return doubleAlphabet

def getMessage():
    stringToEncrypt = input("Please enter a message to encrypt: ")
    return stringToEncrypt

def getCipherKey():
    shiftAmount = input("Please enter a key (whole number from 1-25): ")
    return shiftAmount
    
def encryptMessage(message, cipherKey, alphabet):
    encryptedMessage = ""
    uppercaseMessage = ""
    uppercaseMessage = message.upper()
    for currentCharacter in uppercaseMessage:
        position = alphabet.find(currentCharacter)
        newPosition = position + int(cipherKey)
        if currentCharacter in alphabet:
            encryptedMessage = encryptedMessage + alphabet[newPosition]
        else:
            encryptedMessage = encryptedMessage + currentCharacter
    return encryptedMessage

def decryptMessage(message, cipherKey, alphabet):
    decryptKey = -1 * int(cipherKey)
    return encryptMessage(message, decryptKey, alphabet)    
    
def runCaesarCipherProgram():
    myAlphabet="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
    print(f'Alphabet: {myAlphabet}')
    myAlphabet2 = getDoubleAlphabet(myAlphabet)
    print(f'Alphabet2: {myAlphabet2}')
    myMessage = getMessage()
    print(myMessage)
    myCipherKey = getCipherKey()
    print(myCipherKey)
    myEncryptedMessage = encryptMessage(myMessage, myCipherKey, myAlphabet2)
    print(f'Encrypted Message: {myEncryptedMessage}')
    myDecryptedMessage = decryptMessage(myEncryptedMessage, myCipherKey, myAlphabet2)
    print(f'Decypted Message: {myDecryptedMessage}')
    
runCaesarCipherProgram()
```

**Yes, it's simple.** **Yes, it's basic.** But this is where I started.

## 📚 What This Simple Program Taught Me
1. **My first `for` loop** - understanding iteration
2. **My first `if/else` logic** - making decisions in code  
3. **Character manipulation** - using `ord()` and `chr()`
4. **Problem-solving** - figuring out the "wrap-around" from Z to A
5. **Debugging** - fixing my first `IndentationError` and `SyntaxError`
6. **The satisfaction** - seeing my code actually work for the first time

## 🚀 The Journey This Started
After getting this program to work, I started asking:
- How does **real-world** encryption actually work?
- How do companies like **AWS** protect data at scale?
- What would it take to build **actual security tools**?

That curiosity became my roadmap:
## 🚀 My Learning Journey

**Oct 2025:** Discovered cloud → Joined AWS re/Start  
**Nov 2025:** Started Python → Built this Caesar Cipher  
**Dec 2025:** Graduated AWS re/Start → Learned AWS core services  
**Jan 2026:** Focusing on security → Building cloud security labs  
**Now:** Preparing for AWS certifications → Targeting Cloud Security roles


## 🔐 Connecting Classroom to Cloud
| **This Classroom Project** | **Real AWS Security** | **What I Now Understand** |
|----------------------------|-----------------------|---------------------------|
| My simple shift key (3) | AWS KMS Customer Master Keys | Keys must be managed & rotated |
| A-Z character rotation | AES-256 encryption algorithm | Enterprise-grade cryptography |
| Basic `encrypt()` function | AWS KMS `Encrypt` API calls | Programmatic security operations |
| Print to screen | CloudTrail audit logs | Everything must be logged & monitored |
| Keeping my code private | IAM access policies | Principle of least privilege |

## 🛠️ What I'm Building Now
From this starting point, I'm now working on:

### **🔧 AWS Security Hands-on Labs**
- IAM security policies & role-based access
- VPC network segmentation & security groups  
- CloudTrail log analysis & incident response
- Security monitoring with CloudWatch & AWS Config

### **🐍 Python for Security Automation**
- Scripts to audit AWS resources
- Automated security compliance checks
- Incident response playbooks
- Security dashboard development

### **📜 Professional Development**
- AWS Certified Security Specialty preparation
- Building a cloud security portfolio
- Networking with security professionals
- Contributing to open-source security tools

## 👤 About My Journey
I'm **Renaldi**, currently transitioning from **3+ years in banking customer service** to **cloud security**.

**My Background**:  
No formal tech education → Learned everything through online courses, bootcamps, and hands-on projects

**My Approach**:  
Start with fundamentals → Build simple projects → Gradually increase complexity → Connect concepts to real-world applications

**My Mindset**:  
Embrace being a beginner → Document the learning process → Share progress openly → Help others starting their journeys

**Current Status**:  
✅ AWS re/Start Graduate  
✅ Building cloud security portfolio  
✅ Preparing for AWS certifications  
✅ Seeking Cloud Security Analyst / SOC Analyst roles

## 📬 Connect & Follow My Journey
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_With_Me-blue?logo=linkedin)](https://linkedin.com/in/renaldi-tan)
[![GitHub](https://img.shields.io/badge/GitHub-Follow_My_Projects-black?logo=github)](https://github.com/SilentVeil)

**I'm documenting my entire career transition** - the successes, the challenges, and the lessons learned.

---
*"The expert in anything was once a beginner. This code represents my beginning."*

*"Security is not just about complex tools; it starts with understanding basic principles. This simple Caesar Cipher taught me those principles."*

