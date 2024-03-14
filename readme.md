## Objective

To automate ChargeeBee billing for when an organization adds or reduces licenses. 

## Schedule

This "billing_automation.py" script should be ran on the 1st day of the month.

## Credentials to be added in environment

billing_automation.py
- CHARGEBEE_API_KEY
- CHARGEBEE_SITE

hypercare_api_connection.py
- HYPERCARE_USERNAME
- HYPERCARE_PASSWORD
- HYPERCARE_CLIENT_ID
- HYPERCARE_CLIENT_SECRET

mysql_db_connection.py
- DB_HOST
- DB_USER
- DB_PASSWORD

## How to use the project

The only file to be ran is the "billing_automation.py" script. There are 2 methods that can be used to complete the objective. The default method used is Method #1

Method #1 [PREFERRED/DEFAULT METHOD] <br>
Run the main_api() function to use Hypercare's External API to retrieve an organization's admin data to assess necessary updates needed to be made on ChargeBee 

``` python
if __name__ == '__main__':

    main_api()
```

Method #2 <br>
Run the main_db() function to use DB connection to retrieve an organization's data to assess necessary updates needed to be made on ChargeBee 

``` python
if __name__ == '__main__':

    main_db()
```



