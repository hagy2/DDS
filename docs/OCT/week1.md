---
title: Week 1
parent: October
nav_order: 1
---

# Week 1 Documentation

## Summary of Progress
- Installed and configured essential apps:
  - **PHP**
  - **LDAP**
  - **Borg** (for backup)
- Learned how to create **subdomains** for hosting other apps.
- Attempted to set up **backup processes** (still under review).
- Researched **similar projects** for reference and inspiration.
- Fixed issues with **domain records** (DNS adjustments).
- Added a **Technical Details** section to the documentation for easier access and improved readability.

---

## Research Findings *(Preliminary / Under Review)*
> ⚠️ These findings are **not final**. They are initial observations and insights from reviewing reference projects documentations to guide improvements for YunoHost accessibility and usability. hands on trial will be ddone.

| Platform      | Accessibility Strengths                                                                                                   | Accessibility Weaknesses                                                                                       | Self-Hosting Experience                                                                                 | UI/UX Observations                                                                                       |
| ------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **YunoHost**  | - Centralized app management dashboard <br>- Multilingual support <br>- Clear installation status                        | - Inconsistent keyboard navigation <br>- Screen reader support limited <br>- Some labels missing            | - One-click app installations <br>- Automated upgrades <br>- Active community support                 | - Overlapping categories (Office vs Productivity) <br>- Metadata inconsistent across apps <br>- Navigation dense for first-time users |
| **CHATONS**   | - Privacy-first design <br>- Community-maintained catalog <br>- Basic accessibility: simple layout and clear font        | - Many apps have minimal descriptions <br>- Metadata inconsistent <br>- Accessibility varies by host         | - Installation varies by member (Docker/manual) <br>- Some pre-hosted instances <br>- Decentralized approach | - Simple, uncluttered UI <br>- High contrast readability <br>- Community-driven design                  |
| **Framasoft** | - Clear app descriptions and tutorials <br>- Designed for non-technical users <br>- Responsive layouts                  | - Some apps lack keyboard navigation <br>- Limited advanced configuration <br>- Accessibility varies         | - Mostly manual installation <br>- Emphasis on educational hosted apps <br>- Community support        | - Clean, modern interface <br>- Educational focus <br>- Limited app ecosystem                             |
| **Sandstorm** | - Strong sandboxing <br>- Modern UI <br>- Good keyboard navigation                                                        | - Small app ecosystem <br>- Some apps not fully accessible <br>- Limited community support                     | - Easy deployment via Docker/VM <br>- Security-focused <br>- Documentation limited                     | - Minimalist design <br>- Clear separation of apps and workspace <br>- Focused on power users             |
| **Nextcloud** | - Comprehensive suite (files, calendar, contacts, collaborative editing) <br>- Strong community support                 | - Some keyboard navigation/screen reader issues <br>- Advanced configuration may be complex                  | - Docker, Snap, manual installation options <br>- Extensive documentation                               | - Modern interface <br>- Mobile responsive <br>- Large app ecosystem                                       |
| **Gitea**     | - Lightweight, user-friendly interface <br>- Collaborative features (issues, wikis, pull requests)                        | - Advanced features require configuration <br>- Some accessibility gaps                                      | - Minimal resource requirements <br>- Clear installation guides                                        | - Clean UI <br>- Easy navigation <br>- Suitable for developers                                            |
| **Faveo Helpdesk** | - Feature-rich helpdesk system <br>- Responsive interface                                                               | - Some keyboard navigation issues <br>- Limited accessibility for some UI elements                             | - Easy deployment via Softaculous, AMPPS <br>- Beginner-friendly                                        | - Clean dashboard <br>- Logical workflow <br>- Focus on ticket management                                 |
| **HumHub**    | - Customizable social network <br>- Intuitive interface <br>- Module-based extensions                                     | - Accessibility depends on module/theme <br>- Some elements not fully keyboard accessible                      | - Compatible with shared hosting <br>- Straightforward installation                                     | - Modern layout <br>- Focused on collaboration <br>- Onboarding depends on admin setup                     |

**Key Preliminary Insights**
1. **Accessibility:** Many self-hosted platforms vary in accessibility; consistent ARIA labels, keyboard navigation, and clear metadata are key gaps.  
2. **Self-Hosting:** Docker and automated installations improve usability, but documentation quality affects adoption.  
3. **UI/UX:** Clear categorization, uncluttered dashboards, and descriptive labels improve discoverability.  
4. **Areas for YunoHost:**  
   - Improve metadata standardization for apps.  
   - Enhance keyboard and screen reader accessibility.  
   - Streamline navigation and reduce category overlap.  

> ⚠️ Reminder: This research is **ongoing**. These findings are **preliminary** and may evolve as more projects are reviewed and tested.

---

## Notes
- Focused on stability and ensuring apps integrate properly.  
- Backup process is still being refined (requires testing SSH permissions and automation).  
