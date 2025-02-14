# nsf_cosea
## `filtering_schools.sql`
1. Creates `UNIQUESCHOOLID` in `ga_school_contact_list` and `fte2024-1_enroll-demog_sch`
2. Filters schools by grade range into `filtered_schools`
3. Creates a table for alternative schools `alternative_schools`
4. Removes `alternative_schools` from `filtered_schools`
5. Joins `School Address`, `School City`, `State`, `School ZIPCODE`, `Latitude`, `Longitude` from `ga_school_contact_list` to the new table `tbl_approvedschools`
6. Creates a `schoolgeom` column  that contains the point geom derived from the coordinates