## Confidentiality, Integrity, Availability (CIA)
Confidentiality, Integrity, Availability, or CIA, is a way to think about security trade-offs. This is not a Microsoft model, but is common to all security professionals.

![Confidentiality, Integrity, Availability (CIA)](https://docs.microsoft.com/en-us/learn/wwl-sci/describe-security-concepts-methodologies/media/4-confidentiality-integrity-availability.png)

* ***Confidentiality** refers to the need to keep confidential sensitive data such as customer information, passwords, or financial data. You can encrypt data to keep it confidential, but then you also need to keep the encryption keys confidential. Confidentiality is the most visible part of security; we can clearly see need for sensitive data, keys, passwords, and other secrets to be kept confidential.

* ***Integrity** refers to keeping data or messages correct. When you send an email message, you want to be sure that the message received is the same as the message you sent. When you store data in a database, you want to be sure that the data you retrieve is the same as the data you stored. Encrypting data keeps it confidential, but you must then be able to decrypt it so that it's the same as before it was encrypted. Integrity is about having confidence that data hasn't been tampered with or altered.

* ***Availability** refers to making data available to those who need it. It's important to the organization to keep customer data secure, but at the same time it must also be available to employees who deal with customers. While it might be more secure to store the data in an encrypted format, employees need access to decrypted data.

While all sides of the CIA model are important, they also represent trade-offs that need to be made.
