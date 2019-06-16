---
layout: post
title: What Is Secure By Design?
image: secure-by-design.jpg

---

What is Secure by Design? 🤔🛡️

It's a software development best practice, where the software has been designed from the ground up to be secure.

A good developer must acknowledge that no code is perfect, and vulnerabilities can occur in your code or a third-party library and minimize the risk of such vulnerabilities. I want to share practical tips how to make our JavaScript apps more secure.

![Me Hacking](/images/{{page.image}})

---

1. Always validate user input and avoid writing your custom validation library. A well-tested and actively maintained validation routine, such as [Validator.js](//github.com/chriso/validator.js){: rel="nofollow" }, should be used instead.

2. Always sanitize user input. Sanitization refers to processing submitted data to ensure that it is valid and safe. Good news that Validator.js [supports](//github.com/chriso/validator.js#sanitizers){: rel="nofollow" } sanitization.

3. If you want to show any user-provided data on your web page, then you must filter the data before displaying it. Otherwise, a user can inject malicious code (it's called XSS attack). The library [xss-filters](//github.com/yahoo/xss-filters){: rel="nofollow" } does the job for you.

4. If you allow uploading files, then limit what users are allowed to upload. If a user can upload an avatar, then there is no point in accepting music or large files. If you use Express.js, then [Multer](//bit.ly/unicorn_multer){: rel="nofollow" } library can help you handle uploads securely.

5. Add rate-limiting, because your application could be subject to an attack resulting in a denial of service where real users receive a degraded or unavailable service. A good starting point is [express-rate-limiter](//github.com/nfriedly/express-rate-limit){: rel="nofollow" }.

6. If you create authentication, don't reinvent the wheel. Rely on existing and battle-proven tech, but first understand how it works. Consider using [Passport.js](//passportjs.org){: rel="nofollow" } for authenticating your apps.

7. Pay attention to encrypting sensitive data, such as passwords. Never store passwords in plain text. Besides that, remember to use salt. Without it, a hacker can use so-called Rainbow tables to reverse the passwords. Functions such as [Bcrypt](//github.com/kelektiv/node.bcrypt.js){: rel="nofollow" } allows adding salt to your passwords.

8. Hide error details from clients, otherwise sensitive application details such as server file paths, third-party modules in use, and other internals could be leaked from information found in a stack trace. The best tool to prevent this from happening is a code review. 👀

9. Use code Linters not only for checking your code style but also for finding security issues early in development. I use a [special plugin](//bit.ly/eslink_sec){: rel="nofollow" } for ESLint.

10. Scan your dependencies for vulnerabilities, upgrade old dependencies and replace vulnerable ones with safer alternatives. You can use a free tool [Snyk](//snyk.io){: rel="nofollow" } to scan your dependencies.

Congratulations! You've just become a better developer.

Want to learn more? Here is a [nice article](//bit.ly/unicorn_sec){: rel="nofollow" }.

Want a deep-dive into secure coding? Here is a great free [e-book](//bit.ly/unicorn_scp){: rel="nofollow" }.
