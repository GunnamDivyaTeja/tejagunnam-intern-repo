# Data Privacy Reflection

## Research and Learn

### Key takeaways from Focus Bear's Privacy Policy

- **GDPR:** Focus Bear follows GDPR. It only collects data for a clear purpose and doesn't reuse it for anything else without asking the user first.
- **Encrypted habits:** Habit data is double encrypted. Staff only look at a user's habits if the user reports a problem and asks them to.
- **Sensitive data:** Habits can hint at health conditions or religion, and an optional survey asks about ADHD or autism. Survey data is kept apart from personal details and only looked at as totals.
- **Anonymised data:** Staff only look at anonymised data, and user data isn't shared outside the company except with trusted processors like AWS, Auth0, Stripe and OpenAI.
- **Payments:** Card details are handled by Stripe and never stored by Focus Bear.
- **AI:** OpenAI generates the morning motivational messages and decides which websites to allow during work hours.
- **User rights:** Users can access, correct, delete or export their data by emailing privacy@focusbear.io. Requests are answered within 30 days.
- **Minimum age:** Users must be over 16.

### User data that is considered confidential

- Contact and login details: emails, phone or WhatsApp numbers, login info
- Habit data, which is double encrypted
- Health and religion hints: ADHD or autism survey answers, habits that suggest a condition or religion
- Occupation and survey answers
- Payment and purchase history
- Device info and error logs

### Best practices for handling confidential data

- Access only the data that is needed for my task.
- For any data usage, such as ML model training, anonymise the PII first.
- Only store data in approved places (for example, the company's private S3 bucket with SSE).
- Do not use public AI tools on user data.
- Add API keys, SSH keys and other secrets to `.gitignore` and never commit them to the remote repo.
- Use screen locks and 2FA on accounts for extra protection.
- Report issues and incidents quickly.

### Responding to a suspected data breach

- Report it to the team lead quickly.
- Delete or unsend the message, if possible.
- Rotate any exposed keys and passwords (password, SSH, API).
- Keep notes of what happened and what I did.
- Make sure it does not happen again.

## Reflection

### Steps to ensure data security in my daily tasks

- Lock the screen when I am away from my system.
- Use strong and unique passwords that are not related to any of my personal details.
- Keep my system up to date with the latest patches.
- Do not use or transfer data over public or shared networks.
- Do not share everything with AI tools.

### Storing, sharing and disposing of sensitive information

**Store**
- Keep it only on company-approved systems.
- Don't keep copies on USBs or personal cloud accounts.

**Share**
- Share only with people who need it.
- Use access-controlled links.
- Never share secrets in plain chat or email.

**Dispose**
- Delete files, local copies and downloads once the task is done.
- Revoke access links and tokens I no longer need.

### Common mistakes and how to avoid them

| Mistake | How to avoid it |
|---|---|
| Clicking phishing links | Verify the sender, and don't enter credentials from email links |
| Weak or reused passwords | Use a password manager and turn on 2FA |
| Committing API keys or `.env` files to Git | Use `.gitignore` and check `git diff` before committing |
| Pasting user data or code into public AI tools | Only use approved tools, and anonymise data first |
| Working on public Wi-Fi without protection | Use a VPN or a hotspot |

## Task

**Key learning:** Focus Bear handles sensitive user data like habits, health info (ADHD surveys) and payment details. A small mistake, like pushing a key or pasting data into an AI tool, can expose real users.

**Security measures I will implement:**
- Before every commit, I will run `git status` and `git diff` to check that no `.env` files, API keys, datasets or model files with user data are staged. I will keep these in `.gitignore` in every project.
- I will never use raw user data for training or analysis. I will strip or hash identifiers like emails and names before working with the data.
