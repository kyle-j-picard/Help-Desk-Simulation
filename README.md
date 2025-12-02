# Help-Desk-Simulation
This project demonstrates a fully functional help desk ticketing system built with osTicket in a virtualized environment. It focuses on the practical application of ITIL concepts, including full ticket lifecycle management, SLA compliance, and the creation of user-facing documentation.
osTicket Implementation & Help Desk Simulation

Project Overview

I built a help desk ticketing system to simulate the day-to-day workflow of an IT support specialist. My goal was to move beyond theory and actually practice the "lifecycle" of a support ticket. I wanted to understand how a ticket moves from 'Open' to 'Resolved' while maintaining clear documentation along the way.

This project allowed me to practice Incident Management and Service Level Agreement (SLA) concepts that I learned during my ITIL certification study.

Environment & Technologies

Platform: osTicket (Open Source Ticketing System)

Operating System: Windows 10 (hosted via VirtualBox)

Server Stack: XAMPP (Apache, MySQL, PHP)

Role: Administrator & Support Agent

Key Implementations

1. Installation and Configuration

I started by setting up the prerequisites using XAMPP to create a local web server. Once the database was connected, I installed osTicket. I had to configure the basic system settings, including:

Departments: Created distinct queues for "Support" and "Billing".

SLAs: Set up a standard Service Level Agreement requiring a response within 48 hours.

Help Topics: Configured categories like "Password Reset" and "Hardware Issue" to route tickets automatically.

2. The Ticket Lifecycle

I created a dummy user account to generate test tickets. This helped me see the system from the end-user's perspective.

Intake: I submitted a ticket reporting a "System Slowdown".

Triage: Logging in as an Agent, I categorized the priority level. I assigned the ticket to myself.

Resolution: I added internal notes detailing my troubleshooting steps. This ensures that if another technician looks at the ticket later, they know exactly what I did.

Closing: After verifying the fix, I sent a final response to the user and changed the status to Closed.

Knowledge Base Article

As part of this project, I created a Knowledge Base article to help users solve common issues on their own. This reduces ticket volume for the help desk. Below is the artifact generated during the lab.

KB Article: Troubleshooting "Printer Offline" Status

Description:
This guide addresses the common issue where a network printer appears greyed out or displays an "Offline" status in Windows settings.

Target Audience: All Employees
Difficulty: Beginner

Resolution Steps:

Check Physical Connections
Ensure the printer is plugged into a power source and turned on. If it is a wired printer, check that the Ethernet cable is securely connected to the wall port and the back of the printer.

Restart the Print Spooler Service
Sometimes the Windows service that manages printing gets stuck.

Press the Windows Key + R on your keyboard.

Type services.msc and hit Enter.

Scroll down the list until you find Print Spooler.

Right-click it and select Restart.

Clear the Print Queue
If a document failed to print previously, it might be blocking new jobs. Open your "Printers & Scanners" settings, select your printer, and click "Open Queue." Cancel any old documents listed there.

Verification
Try printing a test page. If the issue persists, please submit a ticket to the IT Support queue with your computer name and the printer model.

Project Takeaways

This lab showed me that technical skills are only half the job. The other half is organization. Keeping accurate notes in a ticket is critical for long-term tracking. If I do not document the solution today, I will have to reinvent the wheel next time the issue happens. This experience has made me much more comfortable with the idea of jumping into a live ticketing queue.
