# API Deployment

---
## Django Settings Best Practices

***Managing Django Settings: Issues***

Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations .


**Sensitive data.** You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

**Sharing settings between team members.** You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.

**Django settings are a Python code.** This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


***Separate settings file for each environment***

This is an extension of the previous approach. It allows you to keep all configurations in VCS and to share default settings between developers.

In this case, you make a settings package with the following file structure :

```
settings/
   ├── __init__.py
   ├── base.py
   ├── ci.py
   ├── local.py
   ├── staging.py
   ├── production.py
   └── qa.py
```

***Pros***

- All environments are in VCS .
- It’s easy to share settings between developers .


***Cons***

- You need to find a way to handle secret passwords and tokens .
- “Inheritance” of settings can be hard to trace and maintain .


***django-environ***

Based on the above, we see that environment variables are the perfect place to store settings.

Writing code using os.environ could be tricky sometimes and require additional effort to handle errors. It’s better to use django-environ instead .


![Django Settings](https://cdn-bpaab.nitrocdn.com/ovmYDbOhMgMfItYufwmmRlRlkhckslfH/assets/static/optimized/rev-02eb3a2/blog/uploads/2019/04/Configuring-Django-Settings_-Best-Practices_long-scaled.jpg)

---
## SSH Tutorial

***What is SSH***

SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client .


***How Does SSH Work***

If you’re using Linux or Mac, then using SSH is very simple. If you use Windows, you will need to utilize an SSH client to open SSH connections. The most popular SSH client is PuTTY .

For Mac and Linux users, head over to your terminal program and then follow the procedure below

The SSH command consists of 3 distinct parts:

> ssh {user}@{host}


Understanding Different Encryption Techniques
The significant advantage offered by SSH over its predecessors is the use of encryption to ensure secure transfer of information between the host and the client. Host refers to the remote server you are trying to access, while the client is the computer you are using to access the host. There are three different encryption technologies used by SSH :

1. Symmetrical encryption .
2. Asymmetrical encryption .
3. Hashing .



![SSH KEY](https://www.hostinger.com/tutorials/wp-content/uploads/sites/2/2017/07/asymmetric-encryption.webp)

---
## Sources and references

- ***[Django Settings Best Practices .](https://djangostars.com/blog/configuring-django-settings-best-practices/)***

- ***[SSH Tutorial .](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)***

- ***[White Noise .](http://whitenoise.evans.io/en/stable/)***

- ***[IaaS .](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)***

- ***[PaaS .](https://en.wikipedia.org/wiki/Platform_as_a_service)***

- ***[CORS .](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)***

---
#### **[Back To Home Page](https://mhmadwrekat.github.io/reading-notes)**

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
