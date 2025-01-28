# Insider Threat Forensics Lab: Investigating Data Breaches at Candy Corp
(Ficticious Organization)

<h2> Lab </h2>
In this lab, I assumed the role of a junior cybersecurity administrator tasked with investigating a critical data breach at Candy Corp. The lab focused on:<br />

-  <b>Forensic Evidence Management</b>: Constructing secure repositories to catalog and analyze logs, emails, and digital artifacts tied to insider threats.<br />
-  <b>Insider Threat Analysis</b>: Identifying collusion between employees leaking proprietary recipes to a competitor, Sugar Corp.<br />
-  <b>Critical Data Recovery</b>: Locating hidden sensitive data, analyzing encrypted files, and isolating evidence tied to stolen intellectual property.<br />
-  <b>Court-Ready Reporting</b>: Compiling a comprehensive evidence dossier to support legal action.<br />

<h2> Step 1: Navigating to secure my workspace </h2>
I navigate into the take_5 directory using the cd command, stepping into my designated forensic workspace. Think of this folder as a virtual crime scene—carefully quarantined to maintain the integrity of the evidence within.
<p align="center">
<img src="https://i.imgur.com/tCyvbDh.png" height="80%" width="90%" alt="Navigating into take_5 Directory"/>

<h2>Step 2: Creating a Case-Specific Investigation Folder </h2>
I use the <b>mkdir</b> command to create the 'Internal_Investigation_Employee_A' folder, following a clear and precise naming convention to ensure it is dedicated exclusively to this suspect's activities. To confirm I am in the correct directory, I run <b>pwd</b>. This verification step is critical— even a minor typo could lead to unintended modifications of live system files. By double-checking, I also ensure the folder was created successfully, avoiding potential errors from working in an incorrect location later on.
<p align="center">
<img src="https://i.imgur.com/9yhbnAI.png" height="80%" width="90%" alt="Creating Internal_Investigation_Employee_A Directory"/>
<img src="https://i.imgur.com/Razgpa2.png" height="80%" width="90%" alt="Navigating into Internal_Investigation_Employee_A Directory"/>

<h2>Step 3: Initializing Core Evidence Files </h2>
I navigate into the dedicated investigation folder to ensure that all files are created in the correct location. Upon discovering that 'web_evidence' is irrelevant (as Candy Corp has no web logs), I delete it using the <b>rm</b> command, adapting my investigation approach as new information arises. I then use <b>ls</b> to list the directory and verify that all necessary files are present. Missing a file at this stage could result in overlooked evidence later in the process.
<p align="center">
<img src="https://i.imgur.com/81pJEFD.png" height="80%" width="90%" alt="Creating multiple files within the current directory"/>
<img src="https://i.imgur.com/60GMuZ0.png" height="80%" width="90%" alt="Deleting a file"/>
<img src="https://i.imgur.com/MthrnaO.png" height="80%" width="90%" alt="Listing all files created"/>

<h2>Step 4: Creating a Second Investigation Directory  </h2>
I use the <b>mkdir</b> command to create the 'Internal_Investigation_Employee_B' folder. This naming convention maintains clarity by distinctly separating the investigation data for each suspect.
<p align="center">
<img src="https://i.imgur.com/YfKG30G.png" height="80%" width="90%" alt="Creating additional directory"/>

<h2>Step 5: Reassigning Evidence with Absolute Paths </h2>
By using <b>mv</b> with absolute paths, I ensure that I'm explicitly targeting the correct file and destination, regardless of my current working directory. This approach prevents accidental misplacement of files during the process.
<p align="center">
<img src="https://i.imgur.com/aRG0CqE.png" height="80%" width="90%" alt="Moving files to another directory"/>

<h2>Step 6: Copying Shared Log Evidence with Absolute Paths </h2>
Using <b>cp</b> with absolute paths ensures I'm referencing the precise source and destination, preventing accidental overwrites or misplacements.
<p align="center">
<img src="https://i.imgur.com/br004a8.png" height="80%" width="90%" alt="Copying files to another directory"/>

<h2>Step 7: Auditing Directories to Verify Evidence Integrity </h2>
Employee A’s folder now contains only 'log_evidence' and 'web_evidence,' as the 'email_evidence' file was moved to Employee B’s directory, based on the updated information that the email leaks are associated with B. Employee B’s folder now holds both 'email_evidence' (moved from A) and 'log_evidence' (copied from A). This ensures that shared logs are preserved for cross-analysis while isolating the email-specific evidence to Employee B's investigation.
<p align="center">
<img src="https://i.imgur.com/7piYWdD.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_A directory"/>
<img src="https://i.imgur.com/JDgdtVE.png" height="80%" width="90%" alt="Checking files in Internal_Investigation_Employee_B directory"/>
<br />

<h2>Step 8: Navigating to the Forensic Workspace </h2>
I use <b>cd</b> to navigate to the centralized forensic workspace, a directory pre-configured by my manager to store all evidence related to the insider threat investigation.
<p align="center">
<img src="https://i.imgur.com/06e9glR.png" height="80%" width="90%" alt="Navigating to oh_henry directory"/>
  
<h2>Step 9: Inspecting Henry’s Files </h2>
I move into the 'Henry' subdirectory using <b>cd</b>, which contains all files extracted from Henry’s workstation. Then, I use <b>ls</b> to list all files within the directory for review.
<p align="center">
<img src="https://i.imgur.com/n1wygxp.png" height="80%" width="90%" alt="Navigating into Henry directory"/>

<h2>Step 10: Previewing Henry’s Files </h2>
By using <b>head</b> with the <b>-n</b> option, I can preview the contents of the files to determine which ones are readable and which are obfuscated.
<p align="center">
<img src="https://i.imgur.com/mMCKPr7.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/PQZ5ndF.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 11: Removing Non-Readable Files </h2>
I use <b>rm</b> to remove all non-readable files from the directory, ensuring that only relevant and accessible evidence remains for analysis.
<p align="center">
<img src="https://i.imgur.com/4KzlGbH.png" height="80%" width="90%" alt="Removing files"/>

<h2>Step 12: Switching Focus to Ruth’s Directory </h2>
I use <b>cd</b> ../Ruth to move up one level to the parent folder and then navigate into Ruth’s dedicated directory. Once there, I use <b>ls</b> to list all files within the directory for review.
<p align="center">
<img src="https://i.imgur.com/5qaLebd.png" height="80%" width="90%" alt="Navigating into Ruth directory"/>

<h2>Step 13: Previewing Ruth’s Files </h2>
Using <b>head</b> with the <b>-n</b> option allows me to preview the files, helping to identify which ones are readable and which are obfuscated.
<p align="center">
<img src="https://i.imgur.com/2PhppWX.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/N4lwWWG.png" height="80%" width="90%" alt="Previewing files"/>
<img src="https://i.imgur.com/rjt8yv9.png" height="80%" width="90%" alt="Previewing files"/>

<h2>Step 14: Removing Non-Readable Files </h2>
I use <b>rm</b> to remove all non-readable files from the directory, ensuring that only relevant, accessible files remain for further analysis.
<p align="center">
<img src="https://i.imgur.com/NllbfJA.png" height="80%" width="90%" alt="Removing files"/>

<h2>Step 15: Navigating to the Central Evidence Directory </h2>
I use <b>cd</b> to navigate to the dedicated investigation directory, a pre-configured folder designed to securely house all evidence and prevent any accidental interaction with live systems.
<p align="center">
<img src="https://i.imgur.com/32lO3Yc.png" height="80%" width="90%" alt="Navigate into working directory"/>

<h2>Step 16: Creating a Dedicated Directory for Combined Evidence </h2>
I use <b>mkdir</b> to create the 'Evidence_for_Authorities' directory. Then, using the <b>ls</b> command, I confirm that the 'Evidence_for_Authorities' directory now exists alongside Henry's and Ruth's directories.
<p align="center">
<img src="https://i.imgur.com/nAgPFK1.png" height="80%" width="90%" alt="Creating a new directory"/>

<h2>Step 17: Navigating through directories to gather potential evidence </h2>
I use the <b>cd</b> command to navigate into the suspected directories, using <b>ls</b> along the way to list the contents and confirm that I am in the correct location.
<p align="center">
<img src="https://i.imgur.com/qoOE7BV.png" height="80%" width="90%" alt="Gathering evidence"/>

<h2>Step 18: Copying files into the ‘Evidence_for_authorities’ directory </h2>
I use the <b>cp</b> command with an absolute path to copy the identified files into the 'Evidence_for_Authorities' directory, ensuring they are safely placed in the correct location. Before executing the command, I preview the text documents using <b>less</b> to confirm that the content is readable. To maintain a clear record, I ensure that the filenames remain unchanged during the copy process. Afterward, I run <b>ls</b> within the directory to verify that the files were successfully copied.
<p align="center">
<img src="https://i.imgur.com/QBAx96T.png" height="80%" width="90%" alt="Copying evidence"/>
<img src="https://i.imgur.com/5qEnpVH.png" height="80%" width="90%" alt="Copying evidence"/>

<h2>Step 19: Concatenating all potential evidence into a single file </h2>
I use the <b>cat</b> command to concatenate all the evidence files into a single file named 'Candy-Evidence.txt' within the 'Evidence_for_Authorities' directory. Afterward, I use <b>head</b> to check the contents of the file, ensuring that the data has merged correctly without any errors.
<p align="center">
<img src="https://i.imgur.com/dNemsV4.png" height="80%" width="90%" alt="Candy-evidence file"/>

<h2>Step 20: Navigating into the working directory </h2>
I use the <b>cd</b> command to enter the designated working directory for this investigation. Then, I use <b>ls</b> to confirm that the expected log files are present before proceeding.
<p align="center">
<img src="https://i.imgur.com/mUVOapR.png" height="80%" width="90%" alt="Navigating into working directory"/>

<h2>Step 21: Counting the number of connections to IP address </h2>
I use the <b>wc -w</b> command to count the number of words in each log file, with each word corresponding to an IP address. This command outputs the total word count for each file, which indicates the number of IP connections per website.
<p align="center">
<img src="https://i.imgur.com/1GwWsHh.png" height="80%" width="90%" alt="Number of connections"/>

<h2>Step 22: Navigating into the working directory </h2>
Using the <b>cd</b> command, I navigate to the designated working directory where the investigation will be conducted.
<p align="center">
<img src="https://i.imgur.com/ixQz8b8.png" height="80%" width="90%" alt="Naviagting into PeanutButtery.net directory"/>

<h2>Step 23: Searching for directories with the word “secret” </h2>
I use the <b>find</b> command to search for directories with 'secret' in their names. This command searches recursively within the specified path, identifying all directories (denoted by <b>-type d</b>) containing 'secret' in their name, regardless of case (using <b>-iname</b>).
<p align="center">
<img src="https://i.imgur.com/57vy0a6.png" height="80%" width="90%" alt="Secret directories"/>

<h2>Step 24: Searching for all files with the word “recipe” </h2>
I use the <b>find</b> command to search for files with 'recipe' in their names. This command searches recursively within the specified directory for files (<b>-type f</b>) that contain 'recipe' in their name, ignoring case sensitivity (<b>-iname</b>).
<p align="center">
<img src="https://i.imgur.com/rdmLOOv.png" height="80%" width="90%" alt="Recipe files"/>

<h2>Step 25: Navigating into the working directory </h2>
I use the <b>cd</b> command to navigate into the designated working directory. Additionally, I run <b>ls</b> to verify that the expected files and folders are present before proceeding.
<p align="center">
<img src="https://i.imgur.com/zxFgl4J.png" height="80%" width="90%" alt="Navigating into working directories"/>

<h2>Step 26: Finding all recipes with guavaberries </h2>
I use the <b>grep -i</b> command to search for the keyword 'guavaberry' across all recipe files in the working directory. This command scans all text files for case-insensitive matches, ensuring that all relevant instances are identified.
<p align="center">
<img src="https://i.imgur.com/goYEI9Z.png" height="80%" width="90%" alt="Search for guavaberries"/>

<h2>Step 27: Navigating into the working directory </h2>
I use the <b>cd</b> command to navigate into the designated working directory, ensuring I'm in the correct location to carry out the investigation.
<p align="center">
<img src="https://i.imgur.com/Bbx5vaB.png" height="80%" width="90%" alt="Navigating into directory"/>

<h2>Step 28: Creating the ‘Sugar_Evidence’ directory </h2>
I use the <b>mkdir</b> command to create a new directory named 'Sugar_Evidence.' After creating the directory, I verify its existence by running <b>ls</b> in the parent directory to ensure it's been created successfully.
<p align="center">
<img src="https://i.imgur.com/1Vb3scV.png" height="80%" width="90%" alt="Creating a new directory"/>

<h2>Step 29: Searching for emails referencing "sugar" </h2>
I use the <b>grep -i</b> command to search for the term 'sugar' within the email files. This performs a case-insensitive search across all email files in the directory and redirects the results, including filenames and matching lines, into a file named 'sugar_email_evidence.' To quantify the occurrences, I pipe the output of the <b>grep</b> command to the <b>wc</b> command to count the number of matches.
<p align="center">
<img src="https://i.imgur.com/dhFI5Aw.png" height="80%" width="90%" alt="List and number of emails"/>

<h2>Step 30: Searching for weblogs referencing Sugar Corp's IP address </h2>
I use the <b>grep -i</b> command to search for the specific IP address associated with Sugar Corp across all weblog files. This command captures all occurrences of the IP address, including the filenames and matching lines, and saves the output to a file named 'web_evidence' for further analysis.
<p align="center">
<img src="https://i.imgur.com/ATCL1Ec.png" height="80%" width="90%" alt="List and number of IPs"/>


<h2>Step 31: Moving the Sugar web evidence file to the ‘Sugar_evidence’ directory </h2>
I use the <b>mv</b> command with an absolute path to move the identified Sugar web evidence file into the 'Sugar_evidence' directory, ensuring proper organization and secure file placement.
<p align="center">
<img src="https://i.imgur.com/79uqE8M.png" height="80%" width="90%" alt="Moving a file"/>


<h2>Step 32: Moving the Sugar email evidence file to the ‘Sugar_evidence’ directory </h2>
I use the <b>mv</b> command with an absolute path to move the Sugar email evidence file into the 'Sugar_evidence' directory, ensuring precise file relocation to the appropriate folder.
<p align="center">
<img src="https://i.imgur.com/BGiptco.png" height="80%" width="90%" alt="Moving a file"/>


<h2>Step 33: Combining both the Sugar email evidence file and the Sugar web evidence file </h2>
I use the <b>cat</b> command to concatenate both files into a single, consolidated file named 'Sugar_evidence_for_authorities.' Afterward, I use <b>cat</b> again to verify the contents of the newly created file in the 'Sugar_evidence' directory, ensuring accuracy and completeness.
<p align="center">
<img src="https://i.imgur.com/OPWtZyh.png" height="80%" width="80%" alt="Combining files"/>
<br />
<br />
