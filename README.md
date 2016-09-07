# SQL-Countries-States-Provinces
An SQL dump of Countries with respective states and provinces.

Original source from https://blueprints.launchpad.net/openobject-server/+spec/countries-states-and-provinces

Normally used for created dependent drop downs, where you select the countries and an option of states or provinces appears.

A simple query to list all countries would be like:

```select * from states_provinces left join countries on states_provinces.country_id = countries.country_id;```

Have fun!
