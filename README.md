# Web-Application-Penetration-Testing-Educational-Platform-Assessment


Summary:
Performed a black-box penetration test on a student organization’s web application to identify and exploit common security flaws. The assessment focused on insecure authentication, access control, and request validation mechanisms. Four critical vulnerabilities were successfully discovered and exploited to demonstrate the potential impact on user privacy and system integrity.

Key Highlights:

🔍 Conducted real-world penetration testing on a live educational platform hosted in a controlled environment.

 SQL Injection (Authentication Bypass)
    • Exploited a login form using ' OR 1=1-- to bypass authentication.
    • Gained unauthorized access as an existing user.

 Insecure Direct Object Reference (IDOR)
    • Accessed and manipulated sensitive user data by modifying studentId in the URL.
    • Demonstrated lack of authorization checks on backend endpoints.

 Cross-Site Request Forgery (CSRF)
    • Created a CSRF attack that silently submitted GPA modification requests.
    • Proved the lack of CSRF token validation and origin checks.

 Broken Access Control (Privilege Escalation)
    • Modified GPA via direct POST requests to /update-gpa endpoint.
    • Demonstrated improper role-based access restrictions.

🛠 Tools & Techniques Used:  manual payload crafting, crafted CSRF HTML, browser developer tools, manipulation of URL.

 Objective: Help developers understand critical security flaws and implement proper mitigations like input validation, token-based request verification, and strict access control.
