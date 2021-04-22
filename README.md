# JmeterPerf
TestRepo

Steps 1: Create a script with HTTP request sampler and listner like Aggregate Report (Sharing RunUsersCMD.jmx file)

Steps 2: In Thread Group make sure you have use function with variable for thread to increase user from command line ${__P(User,1)}

Step 3: To run this script from CMD use this command jmeter -n -t"path\RunUsersCMD.jmx" -l "path\CMDUserPerf.csv"

Step 4 : To set threads from command line use command:

jmeter -n -t"path\RunUsersCMD.jmx" -l "path\CMDUserPerf.csv" -JUser=5 -JRampPeriod=5

Step 5 :  Hit enter

