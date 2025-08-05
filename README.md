# Update README.md with the new content provided by the user
updated_readme = """# My IT Portfolio

👋 Welcome to my professional IT portfolio website.

This site showcases my skills and experience as an **IT Support Specialist**, with hands-on knowledge in areas like:

- Windows Server 2022 (Active Directory, DNS, DHCP, Group Policy)
- Microsoft 365 Administration
- Endpoint management with Microsoft Intune
- Sophos Firewall configuration (VPN, VLAN, rules)
- Microsoft Deployment Toolkit (MDT)
- PowerShell scripting and automation
- Virtualization with VMware ESXi & Hyper-V
- Troubleshooting

---

## 📂 Projects Included

- ✅ Windows Server 2022 Configuration (AD, DNS, DHCP, GPO)
- ✅ Intune Device Management & Security Policies
- ✅ Sophos Firewall VPN & VLAN Setup
- ✅ MDT Deployment Server Configuration
"""

# Write updated README to existing seldeg portfolio folder
updated_readme_path = "/mnt/data/seldeg_portfolio/README.md"
with open(updated_readme_path, "w") as f:
    f.write(updated_readme)

# Create a new ZIP archive with the updated README
updated_zip_path = "/mnt/data/seldeg_portfolio_updated.zip"
shutil.make_archive(updated_zip_path.replace(".zip", ""), 'zip', "/mnt/data/seldeg_portfolio")

updated_zip_path

