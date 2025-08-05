# Create README.md content without contact information
readme_content = """# Seldeg's IT Portfolio

👋 Welcome to my professional IT portfolio website.

This site showcases my skills and experience as an **IT Support Specialist**, with hands-on knowledge in areas like:

- Windows Server 2022 (AD DS, DHCP, DNS, Group Policy)
- Microsoft 365 Administration
- Intune and Endpoint Management
- Sophos Firewall (VPN, VLAN, security rules)
- Microsoft Deployment Toolkit (MDT)
- PowerShell scripting
- VMware ESXi & Hyper-V for lab environments

---

## 📂 Projects Included

- ✅ Windows Server 2022 Configuration
- ✅ Intune Device Management & Policies
- ✅ Sophos Firewall VPN Setup
- ✅ MDT Deployment Server

---

## 🌐 Live Website

You can view the portfolio live at: [https://seldeg.github.io](https://seldeg.github.io)
"""

# Write README.md to the portfolio folder
readme_path = os.path.join(base_path_seldeg, "README.md")
with open(readme_path, "w") as f:
    f.write(readme_content)

# Create a new ZIP file including the README.md
zip_path_seldeg_with_readme = "/mnt/data/seldeg_portfolio_with_readme.zip"
shutil.make_archive(zip_path_seldeg_with_readme.replace(".zip", ""), 'zip', base_path_seldeg)

zip_path_seldeg_with_readme
