# Smart Inbox AI Triager — n8n Agentic Automation

> Automate inbox classification, ticket creation & real-time team notifications

---

### 🧠 Project Overview

The **Smart Inbox AI Triager** automatically classifies incoming emails as
**Support**, **Service/Sales**, or **Spam** using LLM-powered nodes — and routes them accordingly.

It reduces manual workload, speeds up responses, and ensures **no message is missed**.


---

### ✨ Key Features

✔ AI-powered Information Extraction
✔ Auto-classification: *Support / Service / Spam*
✔ Gmail Labeling for traceability
✔ Auto-ticketing in Trello
✔ Slack notifications to correct team
✔ Human-in-the-loop compatible

---

### 🛠️ Architecture & Integrations Used

| Service             | Purpose                               |
| ------------------- | ------------------------------------- |
| Gmail Trigger       | Detect new inbound emails             |
| LangChain LLM Nodes | Extract sender info + classify intent |
| Trello API          | Create support/service tickets        |
| Slack API           | Notify internal teams                 |
| Function/Set Nodes  | Mapping, data handling                |
|                     |                                       |

---

### ⚙️ Workflow Execution Steps

1️⃣ Gmail triggers on new email
2️⃣ Extract sender + details via AI extractor
3️⃣ Classify category via AI classifier
4️⃣ Gmail label applied (Support / Service / Spam)
5️⃣ Route to Trello based on category
6️⃣ Auto-email acknowledgment (Support/Service only)
7️⃣ Slack message with ticket info
8️⃣ Reset & wait for next email


---

### 🔄 AI / Agentic Behavior

| Node                  | Role                                             |
| --------------------- | ------------------------------------------------ |
| Information Extractor | Understands content & extracts structured fields |
| Text Classifier       | Decides ticket category                          |
| Gemini Model          | Language understanding & decision logic          |
|                       |                                                  |

---

### 📸 Screenshots

#### Work Flow

<img width="1776" height="652" alt="Screenshot 2025-11-22 133000" src="https://github.com/user-attachments/assets/ac53a8c9-ada1-4d29-a2bf-06b87c361b2c" />


#### 1️⃣ Email Labeled as Support

<img width="1915" height="920" alt="mail" src="https://github.com/user-attachments/assets/da222e80-7ade-4711-92b5-f5e05c0167f8" />


#### 2️⃣ Acknowledgement Email Sent

<img width="1917" height="915" alt="mail-2" src="https://github.com/user-attachments/assets/6ecc0041-daa5-42f2-902d-a628264be2ce" />


#### 3️⃣ Trello Card Auto-Created

<img width="1916" height="948" alt="fgh" src="https://github.com/user-attachments/assets/1011f4d1-7bd0-4300-b80e-627ea7400f6a" />


#### 4️⃣ Slack Notification with Ticket Link

<img width="1915" height="825" alt="3" src="https://github.com/user-attachments/assets/6f4a43d6-ead9-4f53-b1fa-544969b71dfb" />




---

### 📝 Setup Instructions

| Step | Action                                                  |
| ---- | ------------------------------------------------------- |
| 1    | Import workflow JSON into n8n                           |
| 2    | Configure credentials for Gmail, Trello, Slack & Gemini |
| 3    | Replace placeholder Trello List IDs in Set nodes        |
| 4    | Enable workflow + Gmail Trigger polling frequency       |
|      |                                                         |

> Workflow JSON included:
> **Smart Inbox AI Triager (3).json**
>

---

### 🧪 Testing & Validation

| Case            | Expected Behavior                      |
| --------------- | -------------------------------------- |
| Support Email   | Ticket in Support list + Support reply |
| Service Inquiry | Ticket in Service list + Service reply |
| Spam mail       | Labeled + no reply                     |
| Edge cases      | Graceful handling by extractor         |
|                 |                                        |

---

### 🏁 Conclusion

This workflow **automates** support-based inbox handling using intelligent routing.
It improves customer experience and speeds up internal operations.


---

### 👨‍💻 Author

**Yaswanth Vissamsetty**
📧 [yaswanthvissamsetty@gmail.com](mailto:yaswanthvissamsetty@gmail.com)
Participant — n8n Hackathon

---

## ⭐ How to Support

If you like this project, please ⭐ the repo!

---

### 🔮 Upcoming Enhancements (Optional Add-On Section)

* Priority detection
* Multi-language support
* Improved spam filtering model
* Dashboard for ticket analytics

---

