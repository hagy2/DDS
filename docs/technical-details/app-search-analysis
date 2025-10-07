---
title: YunoHost App Search Analysis
parent: Technical Details
nav_order: 4
---

# Analysis of YunoHost App Search (Demo)

## 1. Categorical Filtering (by category in catalog)

### Synchronization
- **Apps found:** calendars, file sharing, password managers  
- Mostly relevant. Categories are clear.

### Publishing
- **Apps found:** e-commerce, CMS, blog/wiki engines  
- Matches expectations.

### Communication
- **Apps found:** IRC server/client, Matrix clients, chat tools, webmail  
- Some results lack clear descriptions. Slight overlap with *Office* and *Messaging* categories.

### Office
- **Apps found:** note apps, encrypted docs, stock management, diagramming tools, office suites  
- Some apps (comic strip tool, stock management) feel loosely related → may confuse users.

### Productivity and Management
- **Apps found:** finance tools, CRM, database managers, scheduling tools, maps, feedback tools  
- Broad but relevant to productivity.

### Social Media
- **Apps found:** federated social networks, reading/sharing platforms, YouTube alternatives  
- Category appears well-structured.

#### Conclusion on Categories
- Categories work overall but show overlap and inconsistencies:  
  - *Office* vs *Productivity* sometimes redundant  
  - *Communication* contains apps without clear labels  
- Descriptions could be improved to help new users navigate the catalog

---

## 2. Keyword Search (by typing in search bar)

### Email
- **Results:** temporary email tool, invoicing software (with email), groupware  
- Mixed quality; not all results are actual email clients

### Mail
- **Results:** webmail clients, help desk software, newsletter managers  
- More accurate than “email”

### Webmail
- **Results:** only actual webmail clients  
- Very precise

### Calendar
- **Results:** Feber (group calendar)  
- Only one app showed → missing others like Nextcloud

### Events
- **Results:** none  
- Missed expected matches (e.g., calendar/event tools)

### Contacts
- **Results:** SOGo (groupware with contacts)  
- Limited but relevant

### Files / Drive / Storage
- **Files:** mix of file servers + unrelated apps (Hat.sh encryption, MiniDLNA)  
- **Drive:** Nextcloud, ownCloud, Seafile  
- **Storage:** only one app (Armadietto)

### CRM
- **Results:** CiviCRM only  
- Narrow; missed other CRM-like tools

### PKM (Personal Knowledge Management)
- **Results:** none  
- Missing hits like Outline, Cryptpad

### Knowledge
- **Results:** Cryptpad, Outline  
- Accurate but inconsistent with “PKM” label

### Chat / Messaging / Matrix
- **Results:** broad set of clients and servers, including Matrix and XMPP  
- Generally accurate

### Docs
- **Results:** collaborative editors (CodiMD, Collabora)  
- Good match

### Password Manager
- **Results:** KeeWeb only  
- Incomplete; Vaultwarden missing

#### Conclusion on Keyword Search
- Works well for precise keywords (*webmail*, *drive*, *docs*)  
- Generic terms (*email*, *files*, *storage*) return mixed or incomplete results  
- Missing mappings highlight catalog issues:  
  - *Events* → no apps found  
  - *PKM* → no apps found, though apps exist  
  - *Password manager* → only 1 app, incomplete  
- Suggests metadata tags in the app catalog need review and standardization

---

## Overall Findings
1. Categories are broad but useful; some apps are misclassified (*Office* vs *Productivity*)  
2. Keyword search depends heavily on exact terms → synonyms don’t always map  
   - Example: “webmail” works, “email” gives mixed results  
   - “PKM” not recognized, but “knowledge” works  
3. App descriptions are inconsistent; some apps (e.g., IRC clients) lack clear explanations  
4. Users may struggle if they do not know the correct keyword
