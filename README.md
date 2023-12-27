Partner Level Account Health Check
This tool is an executable written in Go and is designed for Windows. It uses the Sophos Central Partner API to query all customers and report back any Account Health Check issues. This produces an healthcheck.csv which can then be used by the Account Health Check Template to produce an actionable report. Each time the health summary is run it will back up the current healthcheck.csv.

Step 1: Extract the Zip file to C:\Health Check

Step 2: Run the Account Health Check Command Line API Call
Open - CMD and navigate to C:\Health Check
Run - sophos_cli.exe
-Enter Central Partner API Creds
Run - sophos_cli.exe healthsummary

Step 3: Open the Account Health Check Template and Enable the Macro.
You can review the macro prior, no code is used, just simple formatting of the document.
Step 4: Save the formatted report to a folder of your choosing.

***The healthcheck.csv will take some time to run depending on the number of customers but will only report on customers with Account Health Check Issues. If the CSV is blank then no customer has an issue that goes against Sophos Best Practices.
