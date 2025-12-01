# kubernetes
first open docker and keep 
next powershell
minikube start
docker login
minikube version
minikube status
kubectl create deployment myngnix --image=ngnix
kubectl get deployment
kubectl get pods
kubectl describe pods 
kubectl expose deployment myngnix --type-Nodeport --port=80 --target-port=80 --name=myngnix
kubectl get service myngnix
kubectl port-forward sevice/myngnix 3080:80
openbrowser and in url 127.0.0.1-3080
....
then open another powershell and 
minikube dashboard
-----------------
# nagioss
open docker desktop
in powershell in adm
docker pull jasonrivers/nagios:latest
docker images
docker run --name nagios4 -d -p 8888:80 jasonrivers/nagios:latest
docker start -ai nagios4
then go localhost:8888
Pranavi ,sonthepranavi9@gmail.com
pranavi944.
Here is your **full SHORT version**, now updated **clearly with what you asked** —
**HOW to create the Payload URL + HOW to add it with menu clicks** 🔥
I placed your request **inside Step 6** neatly.

-----------------

# 🚀 **EXERCISE-1: JENKINS CI/CD USING GITHUB WEBHOOK (FINAL SHORT VERSION + YOUR REQUEST ADDED)**

---

## **STEP 1 — Ngrok Setup**

### ✔ How to know if ngrok already exists

* Search **ngrok.exe** using Windows Search
* If you find → open it
* If ngrok window opens → ngrok already exists

### ✔ Check Jenkins port

* Open browser → type **localhost:8081**
* If Jenkins opens → port = 8081
* If not → try **localhost:8080**

---

## **STEP 2 — Create Ngrok Account**

1. Go to **ngrok.com**
2. Click **Sign Up**
3. Enter:

   * Name: Pranavi
   * Email: [sonthepranavi9@gmail.com](mailto:sonthepranavi9@gmail.com)
   * Password: pranavi944.
4. Dashboard will open

---

## **STEP 3 — Download Ngrok**

1. Click **Download for Windows 64-bit**
2. Extract ZIP
3. Open **ngrok.exe**

---
go to ngrok.com

Login to your account

On left side menu → click Your Authtoken
## **STEP 4 — Add Authtoken**

Dashboard → **Your Authtoken → Copy**
Open ngrok terminal → run:

```
ngrok config add-authtoken <your_token>
```

---

## **STEP 5 — Start tunnel**

Run:

```
ngrok http 8081
```

Copy the generated **https URL** (example: `https://abc123.ngrok-free.dev`)

---

## ✅ **STEP 6 — Add Webhook in GitHub (WITH MENU CLICKS + PAYLOAD URL CREATION)**

### **A) Create the Payload URL**

1. Take the ngrok HTTPS URL (example):
   `https://abc123.ngrok-free.dev`
2. Add this at the end:
   `/github-webhook/`

📌 **Final Payload URL becomes:**

```
https://abc123.ngrok-free.dev/github-webhook/
```

---
-------------------------------------------------------
### **B) Add the Webhook in GitHub (Menu Clicks)**

Follow these clicks:

1. **Open GitHub**
2. Open **your repository**
3. Click **Settings** (left side menu)
4. Click **Webhooks**
5. Click **Add Webhook**

Now fill these:

* **Payload URL:**
  Paste

  ```
  https://abc123.ngrok-free.dev/github-webhook/
  ```

* **Content type:**
  Choose

  ```
  application/json
  ```

* **Select event:**
  Click

  ```
  Just the push event
  ```

* Click **Add Webhook** (green button)

---

## **STEP 7 — Jenkins Trigger**

Jenkins → Job → **Configure → Build Triggers**
✔ Check **GitHub hook trigger for GITScm polling**
→ Save

---

## **STEP 8 — Test**

* Push code to GitHub
* GitHub sends webhook
* Jenkins job runs automatically 🎉

-------------------------------------------------------------------

# 🚀 **EXERCISE-2: JENKINS EMAIL NOTIFICATION (SHORT VERSION)**

Here are the *exact click-wise steps* to set up *Gmail email notifications in Jenkins* — no confusion, just click → click → type.

---

# ✅ *PART 1 — Install Email Extension Plugin*

### *1. Open Jenkins Dashboard*

→ Click *Manage Jenkins*
→ Click system

### *2. Install plugin*

→ Open *Available* tab
→ Search: *Email Extension Plugin*
→ Tick the checkbox
→ Click *Install without restart*
→ After install, click *Go back to Dashboard*

---

# ✅ *PART 2 — Configure Gmail SMTP (Basic E-mail Notification)*

### *1. Go to main settings*

→ Click *Manage Jenkins*
→ Click *Configure System*

### *2. Find: E-mail Notification*

Scroll down until you see *E-mail Notification*

### *3. Fill settings*

→ In *SMTP server* type: smtp.gmail.com
Advanced → Tick *Use SMTP Authentication*
 → *User Name:* your Gmail (example: [pranavi@gmail.com](mailto:pranavi@gmail.com))
 → *Password:* (leave empty for now)
→ Tick *Use SSL*
→ In *SMTP Port* type: 465
→ (Optional) *Reply-To Address:* your email

### *4. Don’t save yet — go to part 3*

---

# ✅ *PART 3 — Create Gmail App Password*
((((Gmail profile --manage google account--security sigin---2 step verifiucation --enter password
 --app passwords  -- app name =jenkins ok 
 click copy paste password )))
### *1. Open Google account*

→ Visit *myaccount.google.com*

### *2. Security*

→ Click *Security*
→ Scroll to *Signing in to Google*
→ Click *2-Step Verification*
→ Turn it ON (enter OTP)

### *3. Create App Password*

→ After 2-step is on, go back to *Security*
→ Click *App Passwords*
→ Enter password
→ In Select app, choose *Other (Custom name)*
→ Type: Jenkins
→ Click *Generate*

### *4. Copy the 16-digit password*

(Google shows a yellow box with 16 letters)
→ Copy it
→ Save in Notepad

---

# ✅ *PART 4 — Add Gmail Credentials to Jenkins*

### *1. Back to Jenkins → Configure System*

→ Go to *E-mail Notification* again

### *2. Add password*

→ Tick *Use SMTP Authentication*
→ *User Name:* your Gmail
→ *Password:* paste the 16-digit app password

### *3. Save*

→ Scroll bottom → Click *Save*

---

# ✅ *PART 5 — Configure Extended Email Notification*

### *1. Go again*

→ Manage Jenkins
→ Configure System
→ Scroll to *Extended E-mail Notification*

### *2. Fill settings*

→ *SMTP Server:* smtp.gmail.com
→ *Port:* 465
→ Tick *Use SSL*
→ *Credentials:*
 → Click *Add*
 → Enter:
  • Username → Gmail
  • Password → 16-digit app password
 → Click *Add* → Select this credential

### *3. Save*

→ Scroll down → *Save*

---

# ✅ *PART 6 — Test Email from Jenkins*

### *1. Test from Basic Email*

→ Manage Jenkins
→ Configure System
→ Go to *E-mail Notification*
→ Click *Test configuration*
→ Enter your email
→ Click *Test*

### *2. Test from Extended Email*

→ Go to *Extended E-mail Notification*
→ Click *Test configuration*
→ Enter your email
→ Click *Test*

📩 You should get an email from Jenkins.

---

# ✅ *PART 7 — Add Email Notification to a Job*

### *1. Open the Job*

→ Go to *Dashboard*
→ Click your job
→ Click *Configure*

### *2. Add post-build action*

→ Scroll to bottom
→ Click *Add Post-build Action*
→ Select *Editable Email Notification*

### *3. Fill job settings*

→ *Project Recipient List:* enter emails
→ *Triggers:* tick *Failure, **Success, or **Always*
→ *Subject/Content:* leave default or edit
→ Click *Save*

---
