# **Ref_XSS Lab**
**A Hands-On DOM Cross-Site Scripting (XSS) Learning Lab**

Access Lab from here : https://giriaryan694-a11y.github.io/Ref_XSS
---

## **📌 What is XSS?**
**Cross-Site Scripting (XSS)** is a security vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users. These scripts can steal cookies, session tokens, or perform actions on behalf of the user.

---

## **🔍 Types of XSS**
This lab **primarily focuses on Reflected XSS**, where malicious scripts are included in a URL and reflected back to the user. However, it also touches on other types:

1. **Stored XSS**
   - Malicious scripts are permanently stored on a server (e.g., in a database).
   - Example: A comment on a blog post that executes when others view it.

2. **Reflected XSS**
   - Malicious scripts are included in a URL and reflected back to the user.
   - Example: A search result page that displays user input unsafely.

3. **DOM-Based XSS**
   - The vulnerability exists in the **Document Object Model (DOM)**.
   - Example: JavaScript dynamically writes user input to the page without sanitization.

---

## **🎯 About This Lab**
This lab is designed to help users **learn and practice Reflected XSS exploitation and prevention** through interactive challenges. It includes **three difficulty levels (Easy, Medium, Hard)** with fun, silly scenarios to keep learning engaging.

---

## **📂 Lab Structure**
Here’s the updated README.md with your requested additions, including a focus on Reflected XSS, cheat sheets, and learning resources:

 Copy# **Ref_XSS Lab**
**A Hands-On Reflected Cross-Site Scripting (XSS) Learning Lab**

---

## **📌 What is XSS?**
**Cross-Site Scripting (XSS)** is a security vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users. These scripts can steal cookies, session tokens, or perform actions on behalf of the user.

---

## **🔍 Types of XSS**
This lab **primarily focuses on Reflected XSS**, where malicious scripts are included in a URL and reflected back to the user. However, it also touches on other types:

1. **Stored XSS**
   - Malicious scripts are permanently stored on a server (e.g., in a database).
   - Example: A comment on a blog post that executes when others view it.

2. **Reflected XSS**
   - Malicious scripts are included in a URL and reflected back to the user.
   - Example: A search result page that displays user input unsafely.

3. **DOM-Based XSS**
   - The vulnerability exists in the **Document Object Model (DOM)**.
   - Example: JavaScript dynamically writes user input to the page without sanitization.

---

## **🎯 About This Lab**
This lab is designed to help users **learn and practice Reflected XSS exploitation and prevention** through interactive challenges. It includes **three difficulty levels (Easy, Medium, Hard)** with fun, silly scenarios to keep learning engaging.

---

## **📂 Lab Structure**
```bash
Ref_XSS/
├── easy/
│   ├── index.html
│   ├── level1.html
│   ├── level2.html
│   └── level3.html
├── medium/
│   ├── index.html
│   ├── level1.html
│   ├── level2.html
│   └── level3.html
├── hard/
│   ├── index.html
│   ├── level1.html
│   ├── level2.html
│   └── level3.html
└── README.md
```

---

## **🚀 How to Use This Lab**
1. **Start with Easy Level**
   - Learn basic XSS payloads like `<img src=x onerror=alert('XSS')>`.
   - Understand how user input is reflected in the page.

2. **Move to Medium Level**
   - Practice exploiting XSS in forms, comments, and profile pages.
   - Learn to bypass basic filters and use event handlers.

3. **Tackle Hard Level**
   - Solve challenges requiring creative payloads (e.g., breaking out of HTML attributes).
   - Understand DOM-based XSS and real-world attack scenarios.

---

## **💡 Example Payloads**

| Type               | Example Payload                          |
|--------------------|------------------------------------------|
| Basic Script       | `<script>alert('XSS')</script>`          |
| Image Error        | `<img src=x onerror=alert('XSS')>`       |
| SVG Payload        | `<svg onload=alert('XSS')>`              |
| HTML Attribute     | `<input onfocus=alert('XSS') autofocus>` |
| JavaScript URI     | `<a href="javascript:alert('XSS')">Click</a>` |

---

## **📜 XSS Cheat Sheet**
For a comprehensive list of XSS payloads and techniques, check out:
🔗 [PortSwigger XSS Cheat Sheet](https://portswigger.net/web-security/cross-site-scripting/cheat-sheet)

---

## **🛡️ How to Prevent XSS**
1. **Input Sanitization**
   - Use libraries like **DOMPurify** to sanitize user input.
   - Escape HTML entities (`&lt;`, `&gt;`, `&quot;`).

2. **Content Security Policy (CSP)**
   - Restrict sources of scripts, styles, and other resources.
   - Example: `Content-Security-Policy: script-src 'self'`

3. **Use Safe APIs**
   - Prefer `textContent` over `innerHTML`.
   - Avoid `eval()` and `document.write()`.

4. **HTTP-only Cookies**
   - Prevent JavaScript from accessing cookies.

---

## **🎓 Learning Outcomes**
- Understand how **Reflected XSS** works and its impact.
- Practice exploiting and fixing XSS vulnerabilities.
- Learn to think like an attacker and a defender.

---

## **📚 Want to Learn More?**
- **PortSwigger XSS Labs**: [Web Security Academy](https://portswigger.net/web-security/all-labs) (Filter for XSS labs)
- **Google XSS Game**: [XSS Game](https://xss-game.appspot.com/)
- **XSS Labs by Abay**: [XSS Labs](https://xss-labs.abay.sh/xss/)

---

## **📢 Contributing**
Found a bug or want to add a new challenge? Open an issue or submit a pull request!

---

## **📜 License**
This project is licensed under the **MIT License**.

---

**Happy Hacking! 🚀** Let’s make the web safer, one XSS challenge at a time.
