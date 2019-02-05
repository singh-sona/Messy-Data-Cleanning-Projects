# Initial Data Exploration and Cleaning projects

![Screenshot Post Page](/img/glass_cleaning.jpg)
 
| Number        | Project Name                         | Tags   |
| --------------|:-------------------------------------|:------------------------|
|Project 1      | Air bnb user destination prediction  | Exploration, Cleaning, prediction|
|Projcet 2| Under construction| |
|Projcet 3| Under construction| |

### This repository includes projects focused on loading data from different sources, understanding data anomalies and apply cleaning and data-transformation tools

## Project 1: Exploratory Walkthrough and Data Cleaning of Airbnb Dataset
[Section1][1] | [Section2][2] | [Section3][3]
### Aim | About Data Set | Workflow | Solutions

### Aim
Project is split in two sections. <br>
1. First section is aimed to find and understand the possible repurcussions of missing values, erroneous values, skweness, formatting issues, duplicate datapoints etc. in data-set of airbnb users provided by kaggle which consist of multiple features of users with outcomes of its country destinations. 
Find section 1 [here][1]
2. Second section deals with actually applying data cleaning and data-tranformation algorithms to eliminate the anomalies.
Find section 2 [here][2]

### About Data Set

Data Source: [here][4] <br>

In this challenge, you are given a list of users along with their demographics, web session records, and some summary statistics. You are asked to predict which country a new user's first booking destination will be. All the users in this dataset are from the USA. <br>

There are 12 possible outcomes of the destination country: **'US', 'FR', 'CA', 'GB', 'ES', 'IT', 'PT', 'NL','DE', 'AU', 'NDF' (no destination found)**, and 'other'. Please note that 'NDF' is different from 'other' because 'other' means there was a booking, but is to a country not included in the list, while 'NDF' means there wasn't a booking. <br>

The training and test sets are split by dates. In the test set, you will predict all the new users with first activities after 7/1/2014 (note: this is updated on 12/5/15 when the competition restarted). In the sessions dataset, the data only dates back to 1/1/2014, while the users dataset dates back to 2010. <br>

File descriptions:

1. train_users.csv - the training set of users
2. test_users.csv - the test set of users <br>
*id: user id<br>
*date_account_created: the date of account creation<br>
*timestamp_first_active: timestamp of the first activity, note that it can be earlier than date_account_created or date_first_booking because a user can search before signing up <br>
*date_first_booking: date of first booking <br>
*gender <br>
*age <br>
*signup_method <br>
*signup_flow: the page a user came to signup up from <br>
*language: international language preference <br>
*affiliate_channel: what kind of paid marketing <br>
*affiliate_provider: where the marketing is e.g. google, craigslist, other <br>
*first_affiliate_tracked: whats the first marketing the user interacted with before the signing up <br>
*signup_app <br>
*first_device_type <br>
*first_browser <br>
*country_destination: this is the target variable you are to predict <br>
*sessions.csv - web sessions log for users <br>
*user_id: to be joined with the column 'id' in users table <br>
*action <br>
*action_type <br>
*action_detail <br>
*device_type <br>
*secs_elapsed
3. countries.csv - summary statistics of destination countries in this dataset and their locations
4. ge_gender_bkts.csv - summary statistics of users' age group, gender, country of destination
5. sample_submission.csv - correct format for submitting your predictions

### Workflow
1. Because all three files contain data of different year, initial exploratory analysis is performed on train data set with contain data of year 2009 to 2014 and saved as `airbnb_explore.ipynb` file.
2. For cleaning, train and test data sets are concatenated and whole data-set is transformed together and saved as `airbnb_clean.ipynb`
3. Build model to predict the destination countries choosen by user-- under development

### Solutions

* `readme.md`.
* `airbnb_explore.ipynb`
* `airbnb_clean.ipynb`
* `data_set`

[1]: https://github.com/singh-sona/Messy-Data-Cleanning-Projects/blob/master/data%20cleaning.ipynb
[2]: https://github.com/singh-sona/Messy-Data-Cleanning-Projects/blob/master/airbnb_clean.ipynb
[3]: https://github.com/singh-sona/Messy-Data-Cleanning-Projects/edit/master/readme.md
[4]: https://www.kaggle.com/c/airbnb-recruiting-new-user-bookings/data


