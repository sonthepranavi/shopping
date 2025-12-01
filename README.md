# kubernetes
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

---

## **STEP 1 — Gmail Setup**

### Enable 2-Step Verification:

myaccount.google.com → Security → **2-Step Verification → ON**

### Generate App Password:

Security → **App Passwords**
Choose:

* App: **Other > Jenkins-Demo**

Copy the 16-digit password.

---

## **STEP 2 — Install Plugin**

Jenkins → Manage Jenkins → Manage Plugins →
Install **Email Extension Plugin**

---

## **STEP 3 — Global Email Settings**

Manage Jenkins → Configure System

### **E-mail Notification**

* SMTP: smtp.gmail.com
* Auth: ✔
* Username: your Gmail
* Password: app password
* SSL: ✔
* Port: 465

### **Extended Email Notification**

* SMTP: smtp.gmail.com
* Port: 465
* SSL: ✔
* Credentials: Gmail + app password

---

## **STEP 4 — Job Email Setup**

Job → Configure → Post-build Actions →
**Editable Email Notification**

Fill:

* Recipients: your email
* Content Type: text/html
* Trigger: Success / Failure

Save.

---

# 🎯 **RESULT**

Whenever a build happens:

✔ You receive **Build Success** email
❌ You receive **Build Failed** email

---

If you want, I can convert **this final version into a PDF** for printing.
You said:
if ngrok already not  exists then only i should go to step3 right
