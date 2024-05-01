# ANALYSIS OF CLIENT BEHAVIOUR AND CHOOSING MORE PROFITABLE PREPAID PLAN
# Data
(1) Users table (data on users):
> - user_id — unique user identifier
> - first_name — user's name
> - last_name — user's last name
> - age — user's age (years)
> - reg_date — subscription date (dd, mm, yy)
> - churn_date — the date the user stopped using the service (if the value is missing, the calling plan was being used when this database was extracted)
> - city — user's city of residence
> - plan — calling plan name

(2) Calls table (data on calls):
> - id — unique call identifier
> - call_date — call date
> - duration — call duration (in minutes)
> - user_id — the identifier of the user making the call

(3) Messages table (data on texts):
> - id — unique text message identifier
> - message_date — text message date
> - user_id — the identifier of the user sending the text

(4) Internet table (data on web sessions):
> - id — unique session identifier
> - mb_used — the volume of data spent during the session (in megabytes)
> - session_date — web session date
> - user_id — user identifier

(5) Plans table (data on the plans):
> - plan_name — calling plan name
> - usd_monthly_fee — monthly charge in US dollars
> - minutes_included — monthly minute allowance
> - messages_included — monthly text allowance
> - mb_per_month_included — data volume allowance (in megabytes)
> - usd_per_minute — price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)
> - usd_per_message — price per text after exceeding the package limits
> - usd_per_gb — price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)


# Goal
Identifying the telecom package with the greatest revenue potential across diverse target markets by analyzing data and performing statistical hypothesis testing.

# Libraries
*pandas ,matplotlib ,numpy, seaborn, missingno, nltk, scipy*
