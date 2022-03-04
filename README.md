# 6156-PerformanceAP-paper-experiment

Command line options : sqlcheck <options>
   
   -f -file_name          :  SQL file name
   
   -r -risk_level         :  Set of anti-patterns to check
   
                          :  1 (all anti-patterns, default) 
   
                          :  2 (only medium and high risk anti-patterns) 
   
                          :  3 (only high risk anti-patterns) 
   
   -c -color_mode         :  Display warnings in color mode 
   
   -v -verbose            :  Display verbose warnings 
   
   -d -delimiter          :  Query delimiter string (; by default) 
   
   -h -help               :  Print help message 


commands(under windows environment - SQLCheck tool can be found in https://github.com/jarulraj/sqlcheck):

run on the database schema with delimiter as ,

sqlcheck.exe  -delimiter , -f .\schemas\The-History-of-Baseball.sql -v   > .\SQLCheck-results\output_baseball_schema.txt

with default delimiter ;

sqlcheck.exe -f .\schemas\The-History-of-Baseball.sql -v   > .\SQLCheck-results\output_baseball_schema_sepBySemicolon.txt

sqlcheck.exe -f .\queries\query4.sql -v   > .\SQLCheck-results\output_query4.txt


