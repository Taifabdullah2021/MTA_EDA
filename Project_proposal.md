# MTA Project Proposal

<img src="https://imgs.6sqft.com/wp-content/uploads/2018/12/21093044/santas-subway.jpg" width="1000" height="400">

## Project idea

The most 2 popular holidays in the USA are **Christmas and Thanksgiving holidays** (based on [Statista](https://www.statista.com/topics/3216/national-holidays-in-the-us/)) These holidays are celebrated by exchanging gifts, sharing food with all family members and friends. Therefore, people who celebrate them will use subways as an option to reach out to their families and friends.
So, my analysis will be based on how much do these two holidays impact the busyness of all the MTA stations? What are the top 3 busiest MTA stations in Christmas and Thanksgiving?

## Who benefits from analysis 

MTA turnstile stations can benefit from this analysis in:
- Solve the under-staffing problems if exist  
- Prepare for the increase in number of people
- Avoid and prepare for possible accidents

## Dataset description

### **MTA Turnstile Data** ([Source](http://web.mta.info/developers/turnstile.html)) :

The Metropolitan Transportation Authority is North America's largest transportation network, serving a population of 15.3 million people across a 5,000-square-mile travel area surrounding New York City through Long Island, southeastern New York State, and Connecticut.

The MTA network comprises the nation’s largest bus fleet and more subway and commuter rail cars than all other U.S. transit systems combined. The MTA's operating agencies are MTA 
New York City Transit, MTA Bus, Long Island Rail Road, Metro-North Railroad, and MTA Bridges and Tunnels.

### Field Description

| Field Name | Description                                                                     |
|------------|---------------------------------------------------------------------------------|
| C/A        | Control Area (A002)                                                             |
| UNIT       | Remote Unit for a station (R051)                                                |
| SCP        | Subunit Channel Position represents an specific address for a device (02-00-00) |
| STATION    | Represents the station name the device is located at                            |
| LINENAME   | Represents all train lines that can be boarded at this station                  |
| DIVISION   | Represents the Line originally the station belonged to BMT, IRT, or IND         |
| DATE       | Represents the date (MM-DD-YY)                                                  |
| TIME       | Represents the time (hh:mm:ss) for a scheduled audit event                      |
| DESC       | Represent the "REGULAR" scheduled audit event (Normally occurs every 4 hours)   |
| ENTRIES    | The comulative entry register value for a device                                |
| EXITS      | The cumulative exit register value for a device                                 |

### Getting the data for this project:

This analysis will be for the data recorded on **(2019-2020)**, the data will be loaded into a pandas data frame and filtered based on the Date. after that, the analysis will be based on the dates before and after Christmas and Thanksgiving holidays to see the difference between the busyness on the normal days and these 2 holidays. 
The main focus columns will be the differenced entries and exits for each station grouped by the date.

## Tools 

- SQLAlchemy in python (Querying the data)
- Pandas and Numpy (Exploring the data)
- Matplotlib and Seaborn (Visualizing the data)
- Other tools may be used during the execution of the data analysis

## MVP Goal

this project will be delivered at the end of week 2, the project will include the following :

- Final report that include the all the steps I took to finish this project
- Final EDA code
- Data base of the MTA turnstile data
- Presentation explaining the summary of the project 

