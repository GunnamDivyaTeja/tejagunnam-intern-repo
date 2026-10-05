# Cyber Security Guidelines

## Research and Learn

### Common cyber security threats in a remote work environment

- Phishing attacks, like fake login pages and cloned email addresses
- Unsecured home or public Wi-Fi networks
- Compromised credentials because of weak or reused passwords
- Malware from downloads or outdated software
- Lost or stolen devices
- Leaked keys in public repos

### Best practices to keep devices and accounts secure

- Keep the browser, OS and apps up to date
- Use a password manager and 2FA
- Use disk encryption
- Use a company-approved antivirus and firewall
- Only install software from trusted sources

### Why I should lock my computer when I am away

I must lock my laptop whenever I am not in front of it. If it is unlocked, anyone can read, copy or send things as me. It only takes a few seconds for someone to get into my open sessions, chats and credentials.

### Handling phishing attempts and suspicious links

- Check the sender's email address.
- Hover over the link to see where it actually goes.
- Do not open unexpected attachments, in any format.
- Never enter my credentials on a page opened from an email. I will go to the original website directly.
- Tell the team lead and the team about the attempt, so they are aware and can take steps to prevent a data leak.

### Strong passwords and password managers

A password is strong if it has 15 or more characters and is a mix of uppercase letters, lowercase letters, numbers and symbols. It is better to set a different password for every account. That way, if one password gets leaked, the other accounts are still safe.

It is hard to remember many different passwords, and it is easy to forget one or mix them up. A password manager solves this because it creates and stores all of them, and I only have to remember one master password. The password manager itself is protected with the master password and 2FA.

### Why 2FA is important

2FA adds another layer of security to an account. Even if an attacker gets my password, they cannot log in without the 6 digit code, which only I can see. It should be enabled on every account that supports it, using an authenticator app like Google Authenticator or Microsoft Authenticator.

## Reflection

### Security measures I follow now, and where I can improve

What I already do:

- Screen lock with a password or PIN
- 2FA on GitHub, email and Discord
- Unique passwords for my important accounts
- Regular OS and browser updates
- Scoped, short-lived tokens

Where I can improve:

- Use a password manager for all my accounts (I have started using Proton Pass)
- Turn on 2FA everywhere it is offered
- Shorten my auto-lock time
- Avoid using public Wi-Fi

### Making secure behaviour a habit

- Use a password manager with 2FA enabled, and not save passwords anywhere else
- Keep the screen auto-lock time as short as possible
- Turn on automatic updates
- Keep a `.gitignore` template so that I do not commit secrets by mistake

### Steps to keep my passwords and accounts secure

- Use a password manager (Proton Pass) to create and store a long, unique password for every account, and to store API keys
- Turn on 2FA for GitHub, email and Discord, using an authenticator app instead of SMS where possible
- Save the 2FA backup codes somewhere safe
- Never share passwords over chat or email
- Not stay logged in on shared devices

### What I would do if I suspected a security breach

1. Change the password right away and sign out of all sessions.
2. Revoke any tokens, keys or app access linked to the account.
3. Check recent activity (logins, commits, messages) to see what was touched.
4. Report it to the team lead right away, with what happened and when.
5. Check other accounts that used the same password, and change those too.

## Task

- My work accounts have strong passwords and 2FA enabled.
- I am using Proton Pass as my password manager.
- My laptop and phone are set to lock automatically when I am away.

### One new cyber security habit

I will lock my screen (Win + L) every time I step away from my laptop, even for a minute. I have also set it to auto-lock after 2 minutes as a backup.
