# AI_MasterClass

**AI Model Training for Document Intelligence Resources**
---
### **Why Document Intelligence?**
- **Real-Life Examples**:
  - Automatically extracting totals from receipts.
  - Sorting emails into spam/inbox.
  - Digitizing handwritten notes.
- **Impact**: Saves time, reduces errors, and unlocks insights from unstructured data.
---
### **Supervised Dataset**

```csv
text,label
"Invoice #INV-2023-001\nDate: 2023-10-05\nTotal Due: $450.00\nDue Date: 2023-10-20",invoice
"Service Invoice\nClient: ABC Corp\nAmount: $1,200.00\nPayment Terms: Net 30",invoice
"Receipt #RC-9876\nDate: 2023-10-05\nTotal Paid: $75.50\nPayment Method: Credit Card",receipt
"Coffee Shop Receipt\nTotal: $4.99\nThank you for your purchase!",receipt
"Subject: Meeting Reminder\nHi Team, don't forget the 2 PM meeting today. Best, John",email
"Urgent: Project Deadline Extended\nNew deadline: November 15th. Regards, Manager",email
"Monthly Sales Report\nOctober 2023\nTotal Sales: $50,000\nTop Product: Widget X",report
"Annual Financial Summary 2023\nRevenue: $1.2M\nExpenses: $900K\nNet Profit: $300K",report
"Service Agreement\nParties: XYZ Corp & Client\nTerm: 12 months\nSignatures: [Signature Block]",contract
"Employment Contract\nPosition: Software Engineer\nStart Date: 2024-01-01\nSalary: $85,000",contract
"Project Invoice\nProject ID: PROJ-456\nTotal: $3,000.00\nStatus: Pending",invoice
"Q3 Marketing Report\nHighlights: Increased engagement by 20%",report
```
---

### **Unsupervised Dataset**
Here’s what the input data might look like **without labels** for unsupervised learning:  
```text
1. "Invoice #INV-2023-005\nDate: 2023-11-10\nTotal Due: $1,000.00\nDue Date: 2023-11-30"
2. "Coffee Shop Receipt\nTotal: $12.75\nPayment Method: Cash\nThank you!"
3. "Subject: Project Update\nHi Team, please review the attached report. Best, Sarah"
4. "Q4 Financial Report\nRevenue: $2.5M\nExpenses: $1.8M\nNet Profit: $700K"
5. "Service Agreement\nClient: XYZ Corp\nTerm: 6 months\nSignatures: [Signed]"
```
---

### **Reinforcement Learning Dataset**
```csv
document,target_index
"Invoice|ID|INV-768|Date|2023-10-05|Total|$500",2
"Receipt|ID|RC-2023|Shop|CoffeeCo|Amount|$8.99",2
"Contract|Client|ABC Corp|SignDate|2023-11-01|Expiry|2025",6
"PO|PO-12345|Vendor|TechSupply|Date|2023-09-15|Cost|$1200",6
"Report|Title|Q4-Sales|Author|John|Total|$50K",5
```
---
```
---
### **Tools & Requirements**
- **`requirements.txt`**:
  ```txt
  numpy==1.21.5
  pandas==1.3.5
  scikit-learn==1.0.2
  matplotlib==3.5.1
  gym==0.26.2
  ```
- **Tools**: Jupyter Notebook, Google Colab, VS Code.

---
