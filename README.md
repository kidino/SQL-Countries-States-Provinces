# SQL Countries States Provinces
An SQL dump of Countries with respective states and provinces.

Original source is in XML format from https://blueprints.launchpad.net/openobject-server/+spec/countries-states-and-provinces

I thought I'd make an SQL version. You normally use this for creating dependent drop downs, where you select a country and an option of states or provinces appears.

A simple query to list all countries would be like:

```
select * 
from states_provinces left join countries 
on states_provinces.country_id = countries.country_id
order by countries.name asc, states_provinces.name asc;
```

Have fun!
